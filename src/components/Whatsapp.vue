<template>
    <p>
        <button @click="whatsappLink(url, title)">Share on whatsapp</button>
    </p>
</template>

<script>
    import objectToGetParams from '../utils/objectToGetParams';
    export default {
      methods: {
        whatsappLink(url, seperator, title) {
          window.open(
            'https://api.whatsapp.com/send' +
              objectToGetParams({
                text: title ? title + separator + url : url
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
      },
      data() {
        return {
          seperator: ' '
        };
      }
    };
</script>
