<template>
  <div id="app">
   
    <filterTabeli></filterTabeli>
    <Tabela/>
  </div>
</template>

<script>
import Tabela from "./components/Tabela"
import FilterTabeli from "./components/Filter"

export default {
  name: "App",
  components: {
    FilterTabeli,
    Tabela,
  },
  mounted(){
    console.log(Wiersz);

  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
