<template>
  <span @click="whatsappLink(url, title)">
    <icon name="brands/whatsapp-square" scale="4"></icon>
  </span>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/whatsapp-square';
  import Icon from 'vue-awesome/components/Icon';
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
    components: {
      Icon
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
