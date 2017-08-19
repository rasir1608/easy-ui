<template>
  <div id="app">
    <!-- <normalButtons></normalButtons>    
    <disabledButtons></disabledButtons>
    <ColorFullButtons></ColorFullButtons>
    <HoverButtons></HoverButtons>  
    <IconButtons></IconButtons>
    <SizeButtons></SizeButtons> -->
    <DisabledRadios></DisabledRadios>
  </div>
</template>

<script>
import Hello from '@/components/Hello.vue'
import normalButtons from '@/components/buttons/normal-buttons.vue'
import disabledButtons from '@/components/buttons/disabled-buttons.vue'
import ColorFullButtons from '@/components/buttons/colorfull-buttons.vue'
import HoverButtons from '@/components/buttons/hover-buttons.vue'
import IconButtons from '@/components/buttons/icon-buttons.vue'
import SizeButtons from '@/components/buttons/size-buttons.vue'
import DisabledRadios from '@/components/form/radios/disabled-radios.vue'

export default {
  name: 'app',
  components:{
    Hello,normalButtons,disabledButtons,ColorFullButtons,HoverButtons,IconButtons,SizeButtons,
    DisabledRadios
  }
}
</script>

<style>
#app {
  font-family: "Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","微软雅黑",Arial,sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
}
</style>
