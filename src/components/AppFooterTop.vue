<script>
export default {
    name: 'AppFooterTop',
    props: {
        footerTopList: Array
    }
    
}
</script>

<template>
    <div id="footer-top">
        <div class="footer-top container">
            <nav class="row">

                <div class="col" v-for="(element, i) in footerTopList" :key="i">
                    <ul v-for="(list, i) in element.list" :key="i">
                        <h4>{{ list.heading }}</h4>
                        <li v-for="(item, i) in list.listItems" :key="i"><a href="#">{{ item }}</a></li>
                    </ul>
                </div>

            </nav>
            <img src="../assets/images/dc-logo-bg.png" alt="">
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

#footer-top {
    background-image: url(../assets/images/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 430px;
    overflow: hidden;
    padding: 2rem 0;
}

.footer-top {
    @include flexbox(baseline, space-between);
}

img {
    width: 50%;
    align-self: flex-start;
}

.row {
    @include flexbox(baseline, flex-start);
    gap: 30px;

    h4 {
        font-size: 1.1rem;
        text-transform: uppercase;
        margin: .8rem 0;
    }

    li {
        padding: .1rem 0;
    }

    a {
        font-size: .8rem;
        color: #959595;
    }
}
</style>