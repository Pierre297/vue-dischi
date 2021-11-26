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
import Song from '@/components/Song.vue'

export default {
  name: 'ListSong',
  components: {
    Song
  },
  data() {
      return {
      songlist: [],
      }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .container {
        width: 70%;
        margin: 20px auto;
    }
    .song-card {
        margin-top: 20px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }
</style>