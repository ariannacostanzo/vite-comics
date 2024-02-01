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
                    <!-- <img v-for="icon in socialIcons" :src="`../assets/images/${icon.url}`" :alt="icon.name"> -->
                    <img v-for="icon in socialIcons" :src="`../assets/images/${icon.url}.png`" :alt="icon.name">
                    <!-- `../assets/images/${icon.url}.png` -->
                </nav>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container {
    max-width: 1200px;
    margin: 0 auto;
}

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
        border: 2px solid #0282f9;
        color: white;
        cursor: pointer;

        &&:hover {
            background-color: #0282f9;
        }
    }

    div {
        display: flex;
        align-items: center;
        gap: 30px;
        color: #0282f9;

        nav {
            display: flex;
            gap: 15px;
        }

    }


}
</style>