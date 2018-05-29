<template>
  <div id="app">
    <img src="./assets/logo.png">
   <vue-social-share></vue-social-share>
  </div>
</template>

<script>
import VueSocialShare from './components/VueSocialShare.vue'

export default {
  name: 'app',
  components: {
    VueSocialShare
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
