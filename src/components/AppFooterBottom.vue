<script>
export default {
    name: 'AppFooterBottom',
    data() {
        return {
            socialIcons: [
                {
                    name: 'facebook',
                    url: 'footer-facebook'
                },
                {
                    name: 'twitter',
                    url: 'footer-twitter'
                },
                {
                    name: 'youtube',
                    url: 'footer-youtube'
                },
                {
                    name: 'pinterest',
                    url: 'footer-pinterest'
                },
                {
                    name: 'periscope',
                    url: 'footer-periscope'
                },
            ]
        }
    },
    mounted() {
        this.socialIcons.forEach((icon)=> {
            console.log(`@/assets/images/${icon.url}.png`)
            
        })
    }
}
</script>

<template>
    <div id="footer-bottom">
        <div class="footer-bottom container">
            <button>Sign-up now!</button>
            <div>
                <h4>FOLLOW US</h4>
                <nav>
                    <!-- non mi funziona il path image -->
                    <!-- <img v-for="icon in socialIcons" :src="`@/assets/images/${icon.url}.png`" :alt="icon.name"> -->
                    <img src="../assets/images/footer-facebook.png" alt="facebook">
                    <img src="../assets/images/footer-twitter.png" alt="twitter">
                    <img src="../assets/images/footer-youtube.png" alt="youtube">
                    <img src="../assets/images/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/images/footer-periscope.png" alt="periscope">
                </nav>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

#footer-bottom {
    background-color: #303030;
}

.footer-bottom {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 2.5rem 0;

    button {
        text-transform: uppercase;
        padding: 15px 20px;
        font-size: 1.1rem;
        background-color: transparent;
        border: 2px solid $blue;
        color: white;
        cursor: pointer;

        &:hover {
            background-color: $blue;
        }
    }

    div {
        display: flex;
        align-items: center;
        gap: 30px;
        color: $blue;

        nav {
            display: flex;
            gap: 20px;
        }

        h4 {
            font-size: 1.3rem;
        }

        img {
            cursor: pointer;
        }

    }


}
</style>