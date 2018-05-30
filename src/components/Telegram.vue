<template>
  <span @click="telegramLink(url, {title})">
    <icon name="brands/telegram-plane" color="#0088cc" :scale="scale"></icon>
  </span>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/telegram-plane';
  import Icon from 'vue-awesome/components/Icon';
  export default {
    name: 'telegram',
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
      },
      scale: {
        required: false,
        type: String
      }
    },
    components: {
      Icon
    }
  };
</script>
