<template>
    <div class="album-card">
        <img :src="info.poster" alt="">
        <h4>{{info.title}}</h4>
        <div class="card-info">{{info.author}}</div>
        <div class="card-info">{{info.genre}}</div>
    </div>

</template>

<script>

    export default {
        name: 'AlbumCard',
        props: {
            info: Object
        },
    }
</script>

<style leng="scss" scoped>
    .album-card {
        background-color: #2E3A46;
    }

    h4 {
        color: #fff;
    }

    img {
        width: 100px;
        height: 100px;
    }
</style>