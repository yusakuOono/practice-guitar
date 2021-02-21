<template>
  <div id="app">
    スケール練習できるよ
    <FirstView/>
  </div>
</template>

<script>
import FirstView from '@/components/FirstView.vue'

export default {
  name: 'App',
  components: {
    FirstView
  }
}
</script>

<style>
html{
  background: #F2EFE4;
}
body{
  margin: 0;
  height: 100vh;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
