<template>
  <span @click="pinterestLink(url)">
    <icon name="brands/pinterest-square" color="#BD081C" :scale="scale"></icon>
  </span>
</template>


<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/pinterest-square';
  import Icon from 'vue-awesome/components/Icon';
  export default {
    name: 'pinterest',
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
