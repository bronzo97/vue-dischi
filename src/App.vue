<template>
  <div id="app">
    <TheHeader></TheHeader>
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
  }
}
</script>

<style lang="scss" scoped>

	@import "assets/styles/main.scss";

</style>
