<template>
  <div class="check-button" :class="{check:isChecked}">
    <img src="../../../assets/img/cart/tick.svg" alt />
  </div>
</template>

<script>
export default {
  name: 'CheckButton',
  data() {
    return {}
  },
  props: {
    isChecked: {
      type: Boolean,
      default: false,
    },
  },
}
</script>

<style scoped>
  .check-button img {
    width: 15px;
    height: 15px;
  }
  .check-button {
    
    border-radius: 50%;
    border: 2px solid #aaa;
  }
  .check {
    border-color: red;
    background-color: red;
  }
</style>
