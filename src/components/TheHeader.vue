<template>
    <header>
            <img src="../assets/img/logo-small.svg" alt="">
            <SearchBar></SearchBar>
    </header>
</template>

<script>
import SearchBar from './SearchBar.vue';


    export default {
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
        img {
            height: 50px;
            width: 50px;
            padding: 10px;
        }

    }
</style>