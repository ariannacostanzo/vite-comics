<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import AppBonus from './components/AppBonus.vue';

  export default {
    name: 'App',
    components: {AppHeader, AppMain, AppFooter, AppBonus}
  }
</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppBonus/>
  <!-- working on footer with branch -->
  <AppFooter/>
</template>

<style>

  * {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  body {
    background-color: #0e0e0e;
    font-family: 'Open Sans', sans-serif;
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