<template>
  <content-body id="vue-content-body"></content-body>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import contentBody from '@/components/content-body.vue';

export default defineComponent({
  name: 'Home',
  components: {
    contentBody,
  },
});
</script>

<style>
#app {
  font-size: 18px;
  font-family: 'Roboto', sans-serif;
  color: blue;
}
</style>
