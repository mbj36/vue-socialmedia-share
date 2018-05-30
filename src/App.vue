<template>
  <div id="app">
    <facebook url="https://google.com" scale="4"></facebook>
    <twitter url="https://github.com/mbj36" title="Check me on Github" scale="4"></twitter>
    <linkedin url="https://google.com" scale="4"></linkedin>
    <telegram url="https://github.com/mbj36" scale="4"></telegram>
    <whats-app url="https://github.com/mbj36" title="Hello" scale="4"></whats-app>
    <pinterest url="https://github.com/mbj36" scale="4"></pinterest>
  </div>
</template>

<script>
  import Facebook from './components/Facebook.vue';
  import Twitter from './components/Twitter';
  import Linkedin from './components/LinkedIn';
  import Telegram from './components/Telegram';
  import WhatsApp from './components/Whatsapp';
  import Pinterest from './components/Pinterest';

  export default {
    name: 'app',
    components: {
      Facebook,
      Twitter,
      Linkedin,
      Telegram,
      WhatsApp,
      Pinterest
    }
  };
</script>

<style>
  #app > span {
    margin: 1em;
  }
</style>


