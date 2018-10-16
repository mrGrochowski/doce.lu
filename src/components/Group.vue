<template>
  <ul class="group"> <!--:id="this._uid" -->
    <li>Persistent</li>
    <li><slot name="group-li"></slot></li>
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
