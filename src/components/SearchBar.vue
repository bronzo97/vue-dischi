<template>
<div class="input-group">
    <select class="custom-select" id="inputGroupSelect04">
        <option selected>Choose...</option>
        <option v-for="album in albumList" :key="album.genre" value="1">{{album.genre}}</option>
    </select>
    <div class="input-group-append">
        <button class="btn btn-outline-secondary" type="button">Button</button>
    </div>
</div>
</template>

<script>


export default {
    props: {
    info: Object
},
    data() {
        return {

        }
    },
    mounted() {

    },
}

</script>

<style lang="scss">
    .input-group {
        justify-content: flex-end;
        padding: 1rem 0;
    }
</style>