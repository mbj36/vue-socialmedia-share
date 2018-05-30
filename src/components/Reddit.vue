<template>
  <span @click="redditLink(url, {title})">
    <icon name="brands/reddit-square" color="#ff4500" :scale="scale"></icon>
  </span>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import Icon from 'vue-awesome/components/Icon';
  import 'vue-awesome/icons/brands/reddit-square';
  export default {
    name: 'reddit',
    methods: {
      redditLink(url, { title }) {
        window.open(
          'https://reddit.com/submit' +
            objectToGetParams({
              url: url,
              title
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
        type: String,
        required: false
      },
      title: {
        type: String,
        required: false
      }
    },
    components: {
      Icon
    }
  };
</script>
