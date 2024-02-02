<script>
import FooterInfo from "./AppElements/FooterInfo.vue";
export default {
    name: 'AppFooterTop',
    props: {
        footerTopList: Array
    },
    components: {FooterInfo}
    
}
</script>

<template>
    <div id="footer-top">
        <div class="footer-top container">
            <nav class="row">

                <FooterInfo :footerTopList="footerTopList"/>

            </nav>
            <figure>
                <img src="../assets/images/dc-logo-bg.png" alt="">
            </figure>

        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

#footer-top {
    background-image: url(../assets/images/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    padding: 2rem 0;
    overflow: hidden;
}

.footer-top {
    @include flexbox(center, space-between);
    
}

figure {
    height: 350px;
    @include flexbox(center, center);
    
}

img {
    width: 500px;
}

.row {
    @include flexbox(baseline, flex-start);
    gap: 30px;
    
}
</style>