<template>
  <div>
  
  <h1>Tabela</h1>

  <ul>
    <wiersz v-for="i in 10" :key='i'></wiersz>
  </ul>

  
  </div>

</template>
<script>
import Wiersz from "./Wiersz"

export default {
  name: "Tabela",
  components : 
  Wiersz
};
</script>
<style scoped>
</style>
