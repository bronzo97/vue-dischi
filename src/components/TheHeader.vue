<template>
    <header>
            <img src="../assets/img/logo-small.svg" alt="">
            <SearchBar :info="album"></SearchBar>
    </header>
</template>

<script>
import SearchBar from './SearchBar.vue';


    export default {
    props: {
        info: Object
    },
    data() {
        return {};
    },
    methods: {},
    components: { SearchBar }
}
</script>

<style lang="scss">
    header {
        background-color: #2E3A46;
        display: flex;
        justify-content: space-between;
        padding: 0 1rem;
        img {
            height: 50px;
            width: 50px;
            padding: 10px;
        }

    }
</style>