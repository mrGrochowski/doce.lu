<template>
  <div>
  
  <h1>Tabela</h1>

  <ul> 
    <wiersz v-for="key in 3" :keys='key' >
      <template slot="to-group-li" v-if="key in {2:'',1:''} "> <wiersz v-for="key in 3" :keys='key'></wiersz></template>
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
