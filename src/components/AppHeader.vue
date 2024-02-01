<script>
  export default {
    name: 'AppHeader',
    data() {
        return {
            nav: [
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
            }],
        }
    }
  }
</script>

<template>
    <header>
        <div class="header container">
            <figure>
                <img src="../assets/images/dc-logo.png" alt="">
            </figure>
            <nav>
                <ul>
                    <li v-for="link in nav"><a :href="link.url" :class="{'active': link.current}">{{ link.text }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>

.container {
    max-width: 1200px;
    margin: 0 auto;
    
} 

header {
    background-color: white;
    padding: 1rem 0;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

img {
    width: 80%;
}

ul{
    display: flex;
    gap: 35px;

    a {
        text-transform: uppercase;
        font-size: .8rem;
        font-weight: 700;
        
    }

}

.active {
    color: #0282f9;
}
</style>