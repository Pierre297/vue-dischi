<template>
  <div id="app">
  </div>
</template>

<script>
import Header from './components/Header.vue'
import ListSong from './components/ListSong.vue'

export default {
  name: 'App',
  components: {
    Header,
    ListSong,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
