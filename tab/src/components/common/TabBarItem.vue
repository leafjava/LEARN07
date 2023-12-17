<template lang="">
  <div class="tab-bar-item" @click="itemClick">
    <div v-if="!isActive" class="icon"><slot name="icon"></slot></div>
    <div v-else class="icon-active"><slot name="icon-active"></slot></div>
    <span :class="{'active':isActive}"><slot name="icon-text"></slot></span>
  </div>
</template>
<script>
export default {
  // data(){
  //   return {
  //     isActive:false
  //   }
  // },
  props:{
    path:String
  },
  methods:{
    itemClick(){
      console.log('click',this.path)
      this.$router.replace(this.path)
    }
  },
  computed:{
    isActive(){
      console.log(this.$route.path)
      return this.$route.path.indexOf(this.path) !== -1;
    }
  }
}
</script>
<style scoped>
  .tab-bar-item{
    flex: 1;
    text-align: center;
    width:30px;
    height:30px;
  }
  .active{
    color:red;
  }
  .icon-text{
  }
</style>