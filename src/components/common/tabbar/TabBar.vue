<template>
  <div id="tab-bar">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'TabBar',
  data() {
    return {}
  },
}
</script>

<style scoped>
#tab-bar {
  height: 49px;
  display: flex;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #f5f5f5;
  box-shadow: 0px -2px 1px rgba(0, 0, 0, 0.1);
}
</style>
