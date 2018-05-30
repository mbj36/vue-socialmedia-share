<template>
  <p>
    <button @click="facebookLink(url)">Share on facebook</button>
  </p>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  export default {
    methods: {
      facebookLink(url) {
        window.open(
          `https://www.facebook.com/sharer/sharer.php` +
            objectToGetParams({
              u: url
            }),
          '__blank'
        );
      }
    },
    props: {
      url: {
        required: true,
        type: String
      }
    }
  };
</script>
