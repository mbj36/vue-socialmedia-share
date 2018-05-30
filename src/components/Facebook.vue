<template>
  <span @click="facebookLink(url)">
    <icon name="brands/facebook" color="#3B5998" :scale="scale"></icon>
  </span>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/facebook';
  import Icon from 'vue-awesome/components/Icon';
  export default {
    name: 'facebook',
    components: {
      Icon
    },
    methods: {
      facebookLink(url) {
        window.open(
          `https://www.facebook.com/sharer/sharer.php` +
            objectToGetParams({
              u: url
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
      scale: {
        required: false,
        type: String
      }
    }
  };
</script>
