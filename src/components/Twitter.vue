<template>
  <span @click="twitterLink(url, {title})">
    <icon name="brands/twitter-square" color="#1DA1F2" :scale="scale"></icon>
  </span>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/twitter-square';
  import Icon from 'vue-awesome/components/Icon';
  export default {
    name: 'twitter',
    methods: {
      twitterLink(url, { title }) {
        window.open(
          'https://www.twitter.com/share' +
            objectToGetParams({
              url: url,
              text: title
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
    }
  };
</script>
