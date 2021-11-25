<template>
  <div class="card">

      <div class="copertina">

      <img :src="card.thumb" :alt="card.type">

      </div>

      <p>{{card.series.toUpperCase()}}</p>
  </div>
</template>

<script>
export default {
    name: 'Card',
    props:{
        card: Object,
    }
}
</script>

<style lang="scss">
@import './src/assets/style/mixins.scss';

.card{
    
    flex-basis: 13%;
    margin: 5px;
    .copertina{
        width: 150px;
        height: 150px;
        overflow: hidden;
    }
    p{
        margin-top: 10px;
        font-size: 11px;
    }
}

</style>