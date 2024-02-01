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
  <AppFooter/>
</template>

<style>
@import './assets/scss/style.scss';
</style>