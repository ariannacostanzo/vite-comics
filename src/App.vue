<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import AppBonus from './components/AppBonus.vue';
  import AppJumbotron from './components/AppJumbotron.vue';
  import { headerNavInfo, comicsCards, buyMerchList, footerBottomSocial, footerTopList } from './assets/data/index.js'

  export default {
    name: 'App',
    components: {AppHeader, AppMain, AppFooter, AppBonus, AppJumbotron},
    data() {
      return {
        headerNavInfo, 
        comicsCards, 
        buyMerchList, 
        footerBottomSocial, 
        footerTopList
      }
    }
  }
</script>

<template>
  <AppHeader :headerNavInfo="headerNavInfo"/>
  <AppJumbotron/>
  <AppMain :comicsCards="comicsCards"/>
  <AppBonus :buyMerchList="buyMerchList"/>
  <AppFooter :footerTopList="footerTopList" :footerBottomSocial="footerBottomSocial"/>
  
</template>

<style>
@import './assets/scss/style.scss';
</style>
