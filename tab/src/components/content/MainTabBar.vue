<template lang="">
  <div class="main-tab-bar">
    <tab-bar>
      <tab-bar-item path='/home'>
        <img slot="icon" src="../../assets/img/tabbar/home.svg">
        <img slot="icon-active" src="../../assets/img/tabbar/home_active.svg">
        <div slot="icon-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path='/category'>
        <img slot="icon" src="../../assets/img/tabbar/category.svg">
        <img slot="icon-active" src="../../assets/img/tabbar/category_active.svg">
        <div slot="icon-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path='/shopCart'>
        <img slot="icon" src="../../assets/img/tabbar/shopcart.svg">
        <img slot="icon-active" src="../../assets/img/tabbar/shopcart_active.svg">
        <div slot="icon-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path='/profile'>
        <img slot="icon" src="../../assets/img/tabbar/profile.svg">
        <img slot="icon-active" src="../../assets/img/tabbar/profile_active.svg">
        <div slot="icon-text">我的</div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>
<script>
import TabBar from "../common/TabBar.vue"
import TabBarItem from "../common/TabBarItem.vue"
export default {
  components:{
    TabBar,
    TabBarItem
  }
}
</script>
<style scoped>
  
</style>