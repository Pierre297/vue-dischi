<template>
<div>
    <select v-model="selectGenre" @change.enter="$emit('inputGenere', selectGenere)">
            <option :value="all">Tutti i generi</option>
            <option :value="rock">Rock</option>
            <option :value="pop">Pop</option>
            <option :value="jazz">Jazz</option>
            <option :value="metal">Metal</option>
        </select>
</div>
</template>

<script>
export default {
  name: 'Filteredgenre',

  data(){
      return{
      selectGenere: "",
      }
  },

}
</script>

<style scoped lang="scss">
    
</style>