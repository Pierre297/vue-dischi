<template>
  <div>
    <span>Select a Genre:</span>
    <select v-model="selectGenere" @change="$emit('inputGenere', selectGenere)">
      <option value="all">Tutti i generi</option>
      <option value="Rock">Rock</option>
      <option value="Pop">Pop</option>
      <option value="Jazz">Jazz</option>
      <option value="Metal">Metal</option>
    </select>
  </div>
</template>

<script>
export default {
  name: "Filteredgenre",

  data() {
    return {
      selectGenere: "",
    };
  },
};
</script>

<style scoped lang="scss">
span {
  color: white;
}
select {
  margin: 30px 20px;
  width: 250px;
  height: 25px;
  border-radius: 15px;
}
</style>