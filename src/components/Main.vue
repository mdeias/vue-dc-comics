<template>
  <main>
      <div class="jumbotrone">
          <img src="../assets/img/jumbotron.jpg" alt="">
      </div>
      <div class="contenitore">
          <h4 class="jumbo-btn"> CURRENT SERIES </h4>
          <Card/>
      </div>
  </main>
</template>

<script>

import Card from '../components/Card.vue';

export default {
    name: 'Main',
    components: {
        Card
    }
}
</script>

<style lang="scss">
@import './src/assets/style/mixins.scss';
main{

    
    height: 500px;
    background-color: #1C1C1C;
    color: white;
    .jumbotrone{
        height: 300px;
        overflow: hidden;
    }
    .contenitore{
        position: relative;
        padding: 50px 0px;
    }
}

</style>