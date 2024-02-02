<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import AppBonus from './components/AppBonus.vue';
  import AppJumbotron from './components/AppJumbotron.vue';

  export default {
    name: 'App',
    components: {AppHeader, AppMain, AppFooter, AppBonus, AppJumbotron}
  }
</script>

<template>
  <AppHeader/>
  <AppJumbotron/>
  <AppMain/>
  <AppBonus/>
  <AppFooter/>
</template>

<style>
@import './assets/scss/style.scss';
</style>\