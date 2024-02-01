<script>
  export default {
    name: 'AppBonus',
    data() {
      return {
        lists: [
          {
            name: 'Digital comics',
            image: 'digital-comics'
          },
          {
            name: 'DC Merchandise',
            image: 'merchandise'
          },
          {
            name: 'Subscription',
            image: 'subscriptions'
          },
          {
            name: 'Comic shop locator',
            image: 'shop-locator'
          },
        ]
      }
    }
  }
</script>

<template>
    <section>
        <ul class="container">
          <li><img src="../assets/images/buy-comics-digital-comics.png" alt=""><a href="">digital comics</a></li>
          <li><img src="../assets/images/buy-comics-merchandise.png" alt=""><a href="">digital comics</a></li>
          <li><img src="../assets/images/buy-comics-subscriptions.png" alt=""><a href="">digital comics</a></li>
          <li><img src="../assets/images/buy-comics-shop-locator.png" alt=""><a href="">digital comics</a></li>
        
         <!-- <li v-for="list in lists"><img :src="`../assets/images/buy-${list.image}.png`" :alt="list.image"><a href="">{{ list.name }}</a></li> -->
        
        </ul>
    </section>
</template>

<style scoped>
  .container {
    max-width: 1200px;
    margin: 0 auto;
    
} 

section {
    color: white;
    background-color: #0282f9;
    font-size: 1.2rem;
    padding: 3rem 0;

    img {
      width: 50px;
    }

    ul {
      display: flex;
      align-items: center;
      justify-content: space-around;
    }

    li {
      display: flex;
      align-items: center;
      gap: 20px;
    }

    a {
      color: white;
    }
}


</style>