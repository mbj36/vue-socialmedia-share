<template>
    <p>
        <button @click="pinterestLink(url)">Share on Pinterest</button>
    </p>
</template>


<script>
    import objectToGetParams from '../utils/objectToGetParams';
    export default {
      methods: {
        pinterestLink(url) {
          window.open(
            'https://pinterest.com/pin/create/button' +
              objectToGetParams({
                url: url
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
