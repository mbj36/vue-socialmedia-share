<template>
  <div id="app">
    <facebook url="https://google.com"></facebook>
    <twitter url="https://github.com/mbj36" title="Check me on Github"></twitter>
    <linkedin url="https://google.com"></linkedin>
  </div>
</template>

<script>
  import Facebook from './components/Facebook.vue';
  import Twitter from './components/Twitter';
  import Linkedin from './components/LinkedIn';

  export default {
    name: 'app',
    components: {
      Facebook,
      Twitter,
      Linkedin
    }
  };
</script>


