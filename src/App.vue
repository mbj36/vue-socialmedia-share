<template>
  <div id="app">
    <facebook :url="url" scale="3"></facebook>
    <twitter :url="url" title="Check me on Github" scale="3"></twitter>
    <linkedin :url="url" scale="3"></linkedin>
    <telegram :url="url" scale="3"></telegram>
    <whats-app :url="url" title="Hello" scale="3"></whats-app>
    <pinterest :url="url" scale="3"></pinterest>
    <reddit :url="url" scale="3" title="My Github"></reddit>
    <google :url="url" scale="3"></google>
    <email :url="url" subject="Hello" scale="3"></email>
  </div>
</template>

<script>
  import Facebook from './components/Facebook.vue';
  import Twitter from './components/Twitter';
  import Linkedin from './components/LinkedIn';
  import Telegram from './components/Telegram';
  import WhatsApp from './components/Whatsapp';
  import Pinterest from './components/Pinterest';
  import Reddit from './components/Reddit';
  import Google from './components/Google';
  import Email from './components/Email';

  export default {
    name: 'app',
    components: {
      Facebook,
      Twitter,
      Linkedin,
      Telegram,
      WhatsApp,
      Pinterest,
      Reddit,
      Google,
      Email
    },
    data() {
      return {
        url: 'https://github.com/mbj36'
      };
    }
  };
</script>

<style>
  #app {
    margin: 7em;
  }
  #app > span {
    margin: 1em;
  }
  .fa-icon {
    fill: currentColor !important;
  }
</style>


