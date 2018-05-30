<template>
  <span @click="googleLink(url)">
    <icon name="brands/google-plus-square" :scale="scale" color="#dd4b39"></icon>
  </span>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/google-plus-square';
  import Icon from 'vue-awesome/components/Icon';
  export default {
    name: 'google',
    methods: {
      googleLink(url) {
        window.open(
          'https://plus.google.com/share' +
            objectToGetParams({
              url: url
            }),
          '__blank'
        );
      }
    },
    props: {
      url: {
        type: String,
        required: true
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
