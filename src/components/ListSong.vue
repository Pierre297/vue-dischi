<template>
  <div class="container">
    <div class="song-card">
        <Song
        v-for="song in songlist"
        :key="song.id"
        :details="song"
        />
    </div>
  </div>
</template>

<script>
import axios from "axios";
import Song from '@/components/Song.vue'

export default {
  name: 'ListSong',
  components: {
    Song
  },
  data() {
      return {
      apiUrl: "https://flynn.boolean.careers/exercises/api/array/music",
      songlist: [],
      }
  },
    //   hook
    created() {
        this.getSongs();

    },
    methods : {
        getSongs() {
            axios
            .get(this.apiUrl)
            .then((result) => {
                this.songlist = result.data.response;
                console.log(result)
            })
        }
    }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .container {
        width: 70%;
        margin: 20px auto;
        background-color: #1e2d3b;
    }
    .song-card {
        margin-top: 20px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }
</style>