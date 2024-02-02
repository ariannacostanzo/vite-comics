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
    methods: {
      createImagePath(item) {
        const path = new URL(`../assets/images/${item}.png`, import.meta.url);
        return path.href
      }
    },
}
</script>

<template>
    <div id="footer-bottom">
        <div class="footer-bottom container">
            <button>Sign-up now!</button>
            <div>
                <h4>FOLLOW US</h4>
                <nav>
                    <img v-for="(icon, i) in socialIcons" :key="i" :src="createImagePath(icon.url)" :alt="icon.name">
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