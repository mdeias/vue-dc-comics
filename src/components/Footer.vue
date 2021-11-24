<template>
  <footer>
      <div class="top">
          <div class="contenitore">ciao</div>
      </div>
      <div class="bottom">
          <div class="contenitore">ciao</div>
      </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss">
@import './src/assets/style/mixins.scss';
footer{
    height: 455px;
    .top{
        height: 70%;
        background-color: green;
    }
    .bottom{
        height: 30%;
        background-color: #303030;
    }
}

</style>