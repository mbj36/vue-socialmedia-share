<template>
  <span @click="whatsappLink(url, title)">
    <icon name="brands/whatsapp-square" color="#34af23" :scale="scale"></icon>
  </span>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/whatsapp-square';
  import Icon from 'vue-awesome/components/Icon';
  export default {
    methods: {
      whatsappLink(url, separator, title) {
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
      },
      scale: {
        required: false,
        type: String
      }
    },
    data() {
      return {
        separator: ''
      };
    }
  };
</script>
