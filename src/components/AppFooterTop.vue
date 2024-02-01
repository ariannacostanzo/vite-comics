<script>
export default {
    name: 'AppFooterTop',
    data() {
        return {
            footerNavbar: [
                {
                    heading: 'Dc comics',
                    listItems: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                },
                {
                    heading: 'Shop',
                    listItems: ['Shop DC', 'Shop DC Collectibles']
                },
                {
                    heading: 'DC',
                    listItems: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscription', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                },
                {
                    heading: 'Sites',
                    listItems: ['Dc', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                },

            ]
        }
    }
}
</script>

<template>
    <div id="footer-top">
        <div class="footer-top container">
            <nav class="row">
                <!-- si potrebbe usare ma non riesco a mettere shop sotto dc comics -->
                <!-- <ul v-for="(ul, i) in footerNavbar" :key="i">
                    <h4>{{ ul.heading }}</h4>
                    <li v-for="(li, i) in ul.listItems" :key="i"><a href="#">{{ li }}</a></li>
                </ul> -->

                <div class="col">
                    <ul>
                        <h4>dc comics</h4>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <ul>
                        <h4>shop</h4>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="col">
                    <ul>
                        <h4>dc</h4>
                        <li><a href="#">Terms of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact us</a></li>
                    </ul>
                </div>
                <div class="col">
                    <ul>
                        <h4>sites</h4>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
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
    display: flex;
    align-items: baseline;
    justify-content: space-between;
}

img {
    width: 50%;
    align-self: flex-start;
}

.row {
    display: flex;
    align-items: baseline;
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