<script>
  import { comicsCards } from "../assets/data";
import ComicsCard from "./AppElements/ComicsCard.vue";
  export default {
    name: 'AppMain',
    props: {
      comicsCards: Array
    },
    components: { ComicsCard }
  }
</script>

<template>
  <main>
    
      <div class="container">
        
          <span class="label">
            current series
          </span>

        <div class="row">
          <comicsCard :comicsCards="comicsCards"/>
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
  @include flexbox(flex-start, flex-start);
  flex-wrap: wrap;
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