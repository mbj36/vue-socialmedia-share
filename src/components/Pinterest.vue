<template>
  <span @click="pinterestLink(url)">
    <icon name="brands/pinterest-square" scale="4"></icon>
  </span>
</template>


<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/pinterest-square';
  import Icon from 'vue-awesome/components/Icon';
  export default {
    methods: {
      pinterestLink(url) {
        window.open(
          'https://pinterest.com/pin/create/button' +
            objectToGetParams({
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
    },
    components: {
      Icon
    }
  };
</script>
