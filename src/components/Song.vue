<template>
<div class="card">
  <div class="songclass">
      <img :src="details.poster" :alt="details.title">
      <h3>{{details.title}}</h3>
      <span>{{details.author}}</span>
      <span>{{details.year}}</span>
  </div>
  </div>
</template>

<script>
export default {
  name: 'Song',
  props: {
      details: Object,
  }

}
</script>

<style scoped lang="scss">
    .songclass{
        text-align: center;
    }
    span{
        display: inline-block;
    }
</style>