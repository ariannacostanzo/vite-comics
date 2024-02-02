<script>
  export default {
    name: 'comicsCard',
    props: {
      comicsCards: Array
    }
  }
</script>

<template>
  <div class="card" v-for="card in comicsCards">
      <figure>
        <img :src="card.thumb" :alt="card.series">
      </figure>
      <p>{{ card.series }}</p>
    </div>
</template>

<style scoped>
    .card {
    flex-basis: calc(100% / 6);
    padding: 1rem 1rem;

      figure {
        height: 170px;
        width: 168px;

      }

      img {
        
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center top;
        
      }

      p {
        font-size: .9rem;
        text-transform: uppercase;
        padding: 1rem 0;
      }

  }


</style>