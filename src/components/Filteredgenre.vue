<template>
<div>
    <select v-model="selectGenre" @change="$emit('inputGenere', selectGenre)">
            <option value="All">Tutti i generi</option>
            <option value="Rock">Rock</option>
            <option value="Pop">Pop</option>
            <option value="Jazz">Jazz</option>
            <option value="Metal">Metal</option>
        </select>
</div>
</template>

<script>
export default {
  name: 'Filteredgenre',

  data(){
      return {
        selectGenere: "",
      }
  },

}
</script>

<style scoped lang="scss">
    
</style>