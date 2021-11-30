<template>
  <div class="header">
    <Filteredgenre @inputGenere="searchGenre"/>
  </div>
</template>

<script>
import Filteredgenre from '@/components/Filteredgenre.vue'

export default {
  name: 'Header',
  components: {
    Filteredgenre,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header{
  background-color: #2e3a46;
  height: 100px;
  
}
</style>
