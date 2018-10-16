<template>
  <ul class="group" :id="'group__'+_uid"> <!--:id="this._uid" -->
    <slot name="group-li"></slot>
  </ul>
</template>
<script>
export default {
  name: "group"
};
</script>
<style scoped>
.group {
  text-align: left;
  padding-left: 15px;
}
</style>
