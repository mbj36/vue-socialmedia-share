<template>
    <p>
        <button @click="telegramLink(url)">Share on Telegram</button>
    </p>
</template>

<script>
    export default {
      methods: {
        telegramLink(url) {
          window.open(
            'https://www.twitter.com/share' +
              objectToGetParams({
                u: url,
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
        }
      }
    };
</script>
