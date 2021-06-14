<template>
    <navbar id="vue-navbar"></navbar>
    <content-body id="vue-content-body"></content-body>
</template>

<script>

import navbar from './components/navbar.vue'
import contentBody from './components/content-body'

export default {
  name: 'App',
  components: {
    navbar,
    contentBody
  }
};
</script>

<style>
#app {
  font-size: 18px;
  font-family: 'Roboto', sans-serif;
  color: blue;
}
</style>