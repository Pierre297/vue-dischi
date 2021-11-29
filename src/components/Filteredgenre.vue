<template>
<div>
    <select name="" id="" v-model="inputGenere">
            <option value="">Tutti i generi</option>
            <option value="">Rock</option>
            <option value="">Pop</option>
            <option value="">Jazz</option>
            <option value="">Metal</option>
        </select>
    <button @click.prevent="selected">select</button>
</div>
</template>

<script>
export default {
  name: 'Filteredgenre',

  data(){
      return{
      inputGenere:"",
      selectGenere: "",
      }
  },
  methods: {
      selected(){
            this.selectGenere = this.inputGenere;
            console.log(this.selectGenere);
        }
  }

}
</script>

<style scoped lang="scss">
    
</style>