<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';

  export default {
    name: 'App',
    components: {AppHeader, AppMain, AppFooter}
  }
</script>

<template>
  <AppHeader/>
  <!-- working on main with branch -->
  <AppMain/>
  <AppFooter/>
</template>

<style>
  body {
    background-color: #0e0e0e;
  }

  /* da mettere nel file scss */
  /* .container {
    max-width: 1200px;
    margin: 0 auto;
  } */

  ul li {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }

  a {
    text-decoration: none;
    color: black;
  }
</style>