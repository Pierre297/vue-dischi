<template>
  <div id="app">
    <div class="header">
      <Filteredgenre @inputGenere="searchGenre" />
    </div>
    <ListSong :selectGenre="selectGenre" />
  </div>
</template>

<script>
import Filteredgenre from "@/components/Filteredgenre.vue";
import ListSong from "./components/ListSong.vue";

export default {
  name: "App",
  components: {
    ListSong,
    Filteredgenre,
  },
  data() {
    return {
      selectGenre: "",
    };
  },
  methods: {
    searchGenre(genre) {
      this.selectGenre = genre;
      console.log(this.selectGenre);
    },
  },
};
</script>

<style lang="scss">
.header {
  background-color: #2e3a46;
  height: 100px;
  display: flex;
  justify-content: end;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #1e2d3b;
}
</style>
