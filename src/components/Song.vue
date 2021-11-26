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
    .card {
        width: calc((100% / 5) - 10px);
        height: 375px;
        
    }
    .songclass{
        text-align: center;
        background-color: #2e3a46;
        height: 350px;

        img {
            width: 150px;
            margin-top: 15px;
        }
        h3 {
            color: white;
        }
        span{
            color: #566b78;
        }
    }
    span{
        display: inline-block;
    }
</style>