<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <main-tab-bar></main-tab-bar>
    <!-- <router-view/> -->
  </div>
</template>

<script>
import MainTabBar from './components/content/MainTabBar'
export default {
  name: 'App',
  components: {
    MainTabBar
  }
}
</script>

<style>

</style>
