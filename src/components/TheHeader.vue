<template>
    <header>
            <img src="../assets/img/logo-small.svg" alt="">
    </header>
</template>

<script>

import axios from "axios";

    export default {
        data() {
            return {
                apiUrl: "https://flynn.boolean.careers/exercises/api/array/music",
            }
        },
        methods: {
            fetchAlbumList() {
                axios.get(this.apiUrl)
                .then((resp) => {
                    resp.dat
                    debugger
                });
            },
        },
        mounted() {
            this.fetchAlbumList();
        }

        }
</script>

<style lang="scss">
    header {
        background-color: #2E3A46;
        img {
            height: 50px;
            width: 50px;
            padding: 10px;
        }

    }
</style>