<template>
<section class="album-list-section">
    <div class="container">
        <div class="row row-cols-5">
            <div class="col"
            v-for="album in albumList" :key="album.title">
                <AlbumCard :info="album"></AlbumCard>
            </div>
        </div>
    </div>
</section>
</template>

<script>
import AlbumCard from './AlbumCard.vue';
import axios from "axios";


    export default {
        name: 'AlbumList',
    data() {
        return {
            apiUrl: "https://flynn.boolean.careers/exercises/api/array/music",
            albumList: [],
        }
    },
    methods: {
        fetchAlbumList() {
            axios.get(this.apiUrl)
            .then((resp) => {
                this.albumList = resp.data.response;

                this.$emit("genresUpdate", this.listaGeneri())

            });
        },
        listaGeneri() {
            const lista = [];

            this.albumList.forEach((album) => {
                if (!lista.includes(album.genre)) {
                    lista.push(album.genre);
                }
            })
            return lista;
        }

    },
    mounted() {
        this.fetchAlbumList();
    },
    components: { 
        AlbumCard
        }
}
</script>

<style leng="scss" scoped>
        .album-list-section {
        background-color: #1E2D3B;
        height: 100%;
        overflow: auto;
    }
</style>