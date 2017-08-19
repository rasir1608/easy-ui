<template>
  <div id="app">
    <normalButtons></normalButtons>    
    <disabledButtons></disabledButtons>
  </div>
</template>

<script>
import Hello from '@/components/Hello.vue'
import normalButtons from '@/components/buttons/normal-buttons.vue'
import disabledButtons from '@/components/buttons/disabled-buttons.vue'

export default {
  name: 'app',
  components:{
    Hello,normalButtons,disabledButtons
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
