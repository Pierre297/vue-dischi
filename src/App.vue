<template>
  <div id="app">
    <Header/>
    <ListSong/>
    <Song/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import ListSong from './components/ListSong.vue'
import Song from '@/components/Song.vue'

export default {
  name: 'App',
  components: {
    Header,
    ListSong,
    Song,
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
