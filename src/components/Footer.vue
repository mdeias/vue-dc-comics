<template>
  <footer>
      <div class="top">
          <div class="contenitore">ciao</div>
      </div>
      <div class="bottom">
          <div class="contenitore">
              <div class="call-to">
              <button> <a href="#">SIGN-UP NOW!</a> </button>
              </div>
              <div class="social">
                  <ul>
                      <li>FOLLOW US</li>
                      <li> <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a> </li>
                      <li> <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a> </li>
                      <li> <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a> </li>
                      <li> <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a> </li>
                      <li> <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a> </li>
                  </ul>
              </div>
          </div>
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
        @include center();
        .contenitore{
            @include center(between);
            .social{
                @include center();
                ul li{
                   display:inline-block;
                   margin-left: 15px;
                   color: #0088FF;
                   font-size: 25px;
                   img{
                       margin-bottom: 5px;
                   }
                }  
            }
            .call-to{
                button{
                    background-color: #303030;
                    padding: 10px 15px;
                    border: 3px solid #0088FF;
                    a{
                        color: white;
                    }
                }
            }
        }
    }
}

</style>