<template>
    <p>
        <button @click="telegramLink(url, {title})">Share on Telegram</button>
    </p>
</template>

<script>
    import objectToGetParams from '../utils/objectToGetParams';
    export default {
      methods: {
        telegramLink(url, { title }) {
          window.open(
            'https://telegram.me/share/' +
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
