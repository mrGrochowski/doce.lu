<template>
  <div>
  
  <h1>Tabela</h1>

  <ul>
    <wiersz v-for="i in 3" :key='i' >
    <template slot="group-slot" v-if="i == 2 "> Coś jeszcze</template>
    </wiersz>
  </ul>

  
  </div>

</template>
<script>
import Wiersz from "./Wiersz"

export default {
  name: "Tabela",
  components : {[Wiersz.name]:Wiersz}
  
};
</script>
<style scoped>
</style>
