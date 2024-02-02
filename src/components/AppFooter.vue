<script>
import AppFooterTop from './AppFooterTop.vue';
import AppFooterBottom from './AppFooterBottom.vue';
  export default {
    name: 'AppFooter',
    components: {AppFooterTop, AppFooterBottom},
    props: {
      footerTopList: Array,
      footerBottomSocial: Array
    }
  }
</script>

<template>
    <footer>
        <AppFooterTop :footerTopList="footerTopList"/>
        <AppFooterBottom :footerBottomSocial="footerBottomSocial"/>
    </footer>
</template>

<style scoped>

@import '../assets/scss/style.scss';

  footer {
    color: white;
  }
</style>