<template>
  <div id="app">
    <facebook url="https://google.com" scale="3"></facebook>
    <twitter url="https://github.com/mbj36" title="Check me on Github" scale="3"></twitter>
    <linkedin url="https://google.com" scale="3"></linkedin>
    <telegram url="https://github.com/mbj36" scale="3"></telegram>
    <whats-app url="https://github.com/mbj36" title="Hello" scale="3"></whats-app>
    <pinterest url="https://github.com/mbj36" scale="3"></pinterest>
    <reddit url="https://github.com/mbj36" scale="3" title="My Github"></reddit>
    <google url="https://github.com/mbj36" scale="3"></google>
    <email url="https://github.com/mbj36" subject="Hello" scale="3"></email>
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
</style>


