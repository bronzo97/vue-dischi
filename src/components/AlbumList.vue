<template>
<section class="album-list-section">
    <div class="container">

        <div class="row-cols-5">
            <div class="col">
                <AlbumCard></AlbumCard>
            </div>
        </div>

    </div>
</section>
</template>

<script>
import AlbumCard from './AlbumCard.vue'

    export default {
    data() {
        return;
    },
    components: { 
        AlbumCard
        }
}
</script>

<style leng="scss" scoped>
        .album-list-section {
        background-color: #1E2D3B;
    }
</style>