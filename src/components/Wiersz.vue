<template>
  <div>
    <li type="1" class="wiersz">Something</li>
    <group v-if="$slots['group-slot']">
      <slot slot="group-li" name="group-slot">
      </slot>
    </group>
  </div>
</template>
<script>
import Group from "./Group.vue"
export default {
  name: "wiersz",
  components:{[Group.name]:Group}
};
</script>
<style scoped>
  .wiersz {text-align:left;}
</style>
