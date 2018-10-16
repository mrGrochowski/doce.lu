<template>
    <li class="wiersz">  {{'unikalna tresc '+_uid}} <a href="!#">🔽</a> <a href="!#">🔼</a> <sup>[id:{{_uid}}]</sup>
    <group v-if="$slots['to-group-li']" >
      <slot slot="group-li" name="to-group-li">
      </slot>
    </group>
    </li>
</template>
<script>
import Group from "./Group.vue"
export default {
  name: "wiersz",
  props:['keys'],
  components:{[Group.name]:Group}
};
</script>
<style scoped>
  .wiersz {text-align:left;}
  a { text-decoration:none; margin-left:10px;}
  sup {color:#aaa; font-style:italic; font-weight: 400; font-family:Tahoma;}
</style>
