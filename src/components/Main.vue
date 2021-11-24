<template>
  <main>
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

    @include center();
    height: 110px;
    background-color: #1C1C1C;
    color: white;

}

</style>