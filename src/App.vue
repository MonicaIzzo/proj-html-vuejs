<script>
// import axios from 'axios';
//import { api } from './data';
//import { store } from './data/store';
import '@fontsource/ubuntu';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: 'Proj HTML Vuejs',
  components: { AppHeader, AppMain, AppFooter },
  data() {
    return {}
  },
  methods: {
  }
};
</script>

<template>
  <!--qui HTML-->
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use 'assets/scss/style.scss' as *;
</style>