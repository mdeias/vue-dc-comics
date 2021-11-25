<template>
  <main>
      <div class="jumbotrone">
          <img src="../assets/img/jumbotron.jpg" alt="">
      </div>
      <div class="contenitore">
          <h4 class="jumbo-btn"> CURRENT SERIES </h4>
          <Card
            v-for="(card, index) in cardList"
            :key="index"
            :card="card"
          />
      </div>
  </main>
</template>

<script>

import Card from '../components/Card.vue';
import cardList from '../assets/data/dc-comics.js'
export default {
    name: 'Main',
    components: {
        Card
    },
     data(){
        return{

        cardList

        }
    }
}    
</script>

<style lang="scss">
@import './src/assets/style/mixins.scss';
main{

    
    min-height: 500px;
    background-color: #1C1C1C;
    color: white;
    .jumbotrone{
        height: 300px;
        overflow: hidden;
    }
    .contenitore{
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        position: relative;
        padding: 50px 0px;
    }
}

</style>