<script>
  export default {
    name: 'AppHeader',
    props: {
        headerNavInfo: Array
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
                    <li v-for="(link, i) in headerNavInfo" :key="i"><a :href="link.url" :class="{'active': link.current}">{{ link.text }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>

@import '../assets/scss/style.scss';

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
        padding: 3.1rem 0;
        
    }

}

.active {
    color: $blue;
    position: relative;

    &::after {
        content: '';
        background-color: $blue;
        width: 100%;
        height: 5px;
        position: absolute;
        bottom: 0;
        left: 0;
    }
}
</style>