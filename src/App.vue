<template>
  <div id="app">
    <div class="toolbar" v-show="isShowToolbar">
      <div class="icom meun"></div>
      <div class="menu_container">
        <router-link tag="div" to="/music"></router-link>
        <router-link tag="div" to="/discover"></router-link>
        <router-link tag="div" to="/friends"></router-link>
      </div>
    </div>
    <router-view></router-view>
    <control-bar :isShow="isShow"></control-bar>
  </div>
</template>

<script>
import controlBar from '@/components/controlBar'
export default {
  data(){
    return{
      isShow: true
    }
  },
  created(){
    
  },
  computed: {
    isShowToolbar(){

    }
  },
  components: {
    controlBar
  }
}
</script>

<style>
  @import "assets/css/reset.css";
  #app #toolbar{

  }
</style>
