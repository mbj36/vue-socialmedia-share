<template>
  <div id="app">
    <facebook url="https://google.com" quote="Hello World"></facebook>
  </div>
</template>

<script>
  import Facebook from './components/Facebook.vue';

  export default {
    name: 'app',
    components: {
      Facebook
    }
  };
</script>


