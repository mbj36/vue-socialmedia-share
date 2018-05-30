<template>
  <p>
    <button @click="twitterLink(url, {title})">Share on twitter</button>
  </p>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  export default {
    methods: {
      twitterLink(url, { title }) {
        window.open(
          'https://www.twitter.com/share' +
            objectToGetParams({
              url: url,
              text: title
            }),
          '__blank'
        );
      }
    },
    props: {
      url: {
        required: true,
        type: String
      },
      title: {
        required: false,
        type: String
      }
    }
  };
</script>
