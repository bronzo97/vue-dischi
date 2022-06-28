<template>
  <div id="app">
    <TheHeader @genresUpdate="onGenresUpdate()"></TheHeader>
    <AlbumList></AlbumList>
  </div>
</template>

<script>

import TheHeader from "./components/TheHeader.vue";
import AlbumList from "./components/AlbumList.vue";

export default {
  name: 'App',
  components: {
    TheHeader,
    AlbumList
  },
  methods: {
    onGenreUpdate(listaGeneri) {
      console.log(listaGeneri)
    }
  }
}
</script>

<style lang="scss" scoped>

	@import "assets/styles/main.scss";

</style>
