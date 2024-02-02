<script>
  export default {
    name: 'AppBonus',
    data() {
      return {
        lists: [
          {
            name: 'Digital comics',
            image: 'buy-comics-digital-comics.png'
          },
          {
            name: 'DC Merchandise',
            image: 'buy-comics-merchandise.png'
          },
          {
            name: 'Subscription',
            image: 'buy-comics-subscriptions.png'
          },
          {
            name: 'Comic shop locator',
            image: 'buy-comics-shop-locator.png'
          },
          {
            name: 'dc power visa',
            image: 'buy-dc-power-visa.svg'
          },

        ]
      }
    },
    methods: {
      createImagePath(item) {
        const path = new URL(`../assets/images/${item}`, import.meta.url);
        return path.href
      }
    },
  }
</script>

<template>
    <section>
        <ul class="container">
         <li v-for="list in lists"><img :src="createImagePath(list.image)" :alt="list.image"><a href="">{{ list.name }}</a></li>
        </ul>
    </section>
</template>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';
// @use '../assets/scss/style.scss'as *

section {
    color: white;
    background-color: $blue;
    font-size: .8rem;
    padding: 3rem 0;

    img {
      height: 50px;
    }

    ul {
      display: flex;
      align-items: center;
      justify-content: space-around;
      gap: 30px;
    }

    li {
      display: flex;
      align-items: center;
      gap: 20px;
    }

    a {
      color: white;
      text-transform: uppercase;
    }
}


</style>