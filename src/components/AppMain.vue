<script>
  export default {
    name: 'AppMain',
    props: {
      comicsCards: Array
    },
  }
</script>

<template>
    <main>
      
        <div class="container">
            <span class="label">
              current series
            </span>

          <div class="row">

            <div class="card" v-for="card in comicsCards">
              <figure>
                <img :src="card.thumb" :alt="card.series">
              </figure>
              <p>{{ card.series }}</p>
            </div>
            
          </div>

          <div class="btn-div">
            <button>LOAD MORE</button>
          </div>

        </div>

    </main>
</template>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

  main {
    color: white;
    font-size: 1.5rem;
    padding: 1.5rem 0;
    background-color: #1c1c1c;
  }

  .label {
    text-transform: uppercase;
    font-size: 1.5rem;
    font-weight: bold;
    background-color: $blue;
    padding: 10px 25px;
    position: relative;
    top: -40px;
    left: 0;
    
  }

  .row {
    @include flexbox(baseline, flex-start);
    flex-wrap: wrap;


    .card {
      flex-basis: calc(100% / 6);
      padding: 1rem 1rem;

      figure {
        height: 170px;
        overflow: hidden;
      }
      img {
        max-width: 100%;
        object-fit: fill; 
        
      }

      p {
        font-size: .9rem;
        text-transform: uppercase;
        padding: 1rem 0;
      }
    }

  }

  .btn-div {
    @include flexbox(center, center);

    button {
      text-align: center;
      padding: 12px 40px;
      background-color: $blue;
      border: 0;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }
  }

  

  
</style>