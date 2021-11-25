<template>
  <section> 
      <div class="contenitore">
          <div>
              <img src="../assets/img/buy-comics-digital-comics.png" alt="">
              <p>DIGITAL COMICS</p>
          </div>
          <div>
              <img src="../assets/img/buy-comics-merchandise.png" alt="">
              <p>DC MERCHANDISE</p>
          </div>
          <div>
              <img src="../assets/img/buy-comics-shop-locator.png" alt="">
              <p>SUBSCRIPTION</p>
          </div>
          <div>
              <img src="../assets/img/buy-comics-subscriptions.png" alt="">
              <p>COMICS SHOP LOCATION</p>
          </div>
          <div>
              <img src="../assets/img/buy-dc-power-visa.svg" alt="">
              <p>DC POWER VISA</p>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Merch'
}
</script>

<style lang="scss">
@import './src/assets/style/mixins.scss';
section{
    @include center();
    height: 150px;
    background-color: #0081FA;
    .contenitore{
        @include center(between);
        div{
            @include center();
            width: 18%;
            img{
                width: 20%;
                margin-right: 10px;
            }
            p{
                
                color: white;
                font-size: 10px;
            }
        }
    }
}
</style>