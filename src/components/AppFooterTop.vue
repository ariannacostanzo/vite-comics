<script>
  export default {
    name: 'AppFooterTop',
    data() {
        return {
            footerNavbar: [
                {
                    heading: 'Dc comics',
                    listItems: ['Characters','Comics','Movies', 'TV', 'Games', 'Videos', 'News']
                },
                {
                    heading: 'Shop',
                    listItems: ['Shop DC','Shop DC Collectibles']
                },
                {
                    heading: 'DC',
                    listItems: ['Terms Of Use','Privacy policy (New)','Ad Choices', 'Advertising', 'Jobs', 'Subscription', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                },
                {
                    heading: 'Sites',
                    listItems: ['Dc','MAD Magazine','DC Kids', 'DC Universe', 'DC Power Visa']
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
            <ul v-for="ul in footerNavbar">
                <h4>{{ ul.heading }}</h4>
                <li v-for="li in ul.listItems"><a href="#">{{ li }}</a></li>
            </ul>
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
    }

    .footer-top {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    img {
        width: 40%;
    }

    .row {
        display: flex;
        align-items: baseline;
        gap: 30px;

        h4 {
            font-size: 1.1rem;
            text-transform: uppercase;
            margin-bottom: .8rem;
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