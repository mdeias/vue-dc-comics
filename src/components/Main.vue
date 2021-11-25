<template>
  <main>
      <div class="jumbotrone">
          <img src="../assets/img/jumbotron.jpg" alt="">
      </div>
      <div class="contenitore">
          <h2> Content goes here </h2>
      </div>
  </main>
</template>

<script>
export default {
    name: 'Main'
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
    
}

</style>