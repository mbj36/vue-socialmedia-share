<template>
    <span @click="emailLink(url, {subject, body})">
        <icon name="envelope-square" :scale="scale" color="#ff4343"></icon>
    </span>
</template>

<script>
    import objectToGetParams from '../utils/objectToGetParams';
    import 'vue-awesome/icons/envelope-square';
    import Icon from 'vue-awesome/components/Icon';
    export default {
      methods: {
        emailLink(url, { subject, body }) {
          window.open(
            'mailto:' +
              objectToGetParams({
                subject,
                body: body || url
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
        },
        subject: {
          required: false,
          type: String
        },
        body: {
          required: false,
          type: String
        }
      },
      components: {
        Icon
      }
    };
</script>
