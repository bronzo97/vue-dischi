<template>
    <div class="album-card">
        <img :src="info.poster" alt="">
        <h5>{{info.title}}</h5>
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
        text-align: center;
        margin: 1rem 0;
    }

    h5 {
        color: #fff;
        text-transform: uppercase;
    }

    img {
        width: 100px;
        height: 100px;
    }
    .card-info {
        font-size: 0.8rem;
    }
</style>