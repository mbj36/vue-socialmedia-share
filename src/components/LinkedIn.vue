<template>
    <p>
        <button @click="linkedinLink(url)">Share on linkedin</button>
    </p>
</template>

<script>
    import objectToGetParams from '../utils/objectToGetParams';
    export default {
      methods: {
        linkedinLink(url) {
          window.open(
            'https://linkedin.com/shareArticle' +
              objectToGetParams({
                mini: true,
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
