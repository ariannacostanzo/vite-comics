<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import AppBonus from './components/AppBonus.vue';
  import AppJumbotron from './components/AppJumbotron.vue';

  export default {
    name: 'App',
    components: {AppHeader, AppMain, AppFooter, AppBonus, AppJumbotron},
    data() {
      return {
          headerNavInfo: [
            {
                text: 'Characters',
                url: '#',
                current: false,
            },
            {
                text: 'Comics',
                url: '#',
                current: true,
            },
            {
                text: 'Movies',
                url: '#',
                current: false,
            },
            {
                text: 'TV',
                url: '#',
                current: false,
            },
            {
                text: 'Games',
                url: '#',
                current: false,
            },
            {
                text: 'Collectibles',
                url: '#',
                current: false,
            },
            {
                text: 'Videos',
                url: '#',
                current: false,
            },
            {
                text: 'Fans',
                url: '#',
                current: false,
            },
            {
                text: 'News',
                url: '#',
                current: false,
            },
            {
                text: 'Shop',
                url: '#',
                current: false,
            }]
      }
    }
  }
</script>

<template>
  <AppHeader :headerNavInfo="headerNavInfo"/>
  <AppJumbotron/>
  <AppMain/>
  <AppBonus/>
  <AppFooter/>
</template>

<style>
@import './assets/scss/style.scss';
</style>