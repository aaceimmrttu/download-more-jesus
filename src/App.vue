<template>
  <navbar id="vue-navbar"></navbar>
  <router-view id="router-view"/>
</template>

<script>
import navbar from './components/navbar.vue';

export default {
  name: 'App',
  components: {
    navbar,
  },
};
</script>

<style>
#app {
  font-size: 18px;
  font-family: 'Roboto', sans-serif;
  color: blue;
}

#vue-navbar {
  margin-top: 5px;
  margin-bottom: 5px;
  height: 4em;
}

#router-view {
  margin-top: calc( 3.5em + 10px);
}
</style>
