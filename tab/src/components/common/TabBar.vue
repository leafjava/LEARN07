<template lang="">
  <div class="tab-bar">
    <slot></slot>
  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped>
  .tab-bar{
    display:flex;
    justify-content: center;
    height:49px;

    position:fixed;
    bottom:49px;
    left:0;
    right:0;
  }
</style>