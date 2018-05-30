<template>
  <span @click="linkedinLink(url)">
    <icon name="brands/linkedin-in" :scale="scale"></icon>
  </span>
</template>

<script>
  import objectToGetParams from '../utils/objectToGetParams';
  import 'vue-awesome/icons/brands/linkedin-in';
  import Icon from 'vue-awesome/components/Icon';
  export default {
    components: {
      Icon
    },
    methods: {
      linkedinLink(url) {
        window.open(
          'https://linkedin.com/shareArticle' +
            objectToGetParams({
              mini: true,
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
    }
  };
</script>
