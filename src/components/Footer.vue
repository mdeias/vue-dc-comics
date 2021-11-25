<template>
  <footer>
      <div class="top">
          <div class="contenitore">
              <div class="dclist">
                  <ul>
                      <li><h6>DC COMICS</h6></li>
                      <li><a href="#">Characters</a></li>
                      <li><a href="#">Comics</a></li>
                      <li><a href="#">Movies</a></li>
                      <li><a href="#">TV</a></li>
                      <li><a href="#">Games</a></li>
                      <li><a href="#">Videos</a></li>
                      <li><a href="#">News</a></li>
                      <li class="shop"><h6>SHOP</h6></li>
                      <li><a href="#">Lorem</a></li>
                      <li><a href="#">Lorem</a></li>
                  </ul>
                  <ul>
                      <li><h6>DC</h6></li>
                      <li v-for="(link, index) in links" :key="index + 'links'"><a href="#">{{link}}</a></li>
                  </ul>
                  <ul>
                      <li><h6>SITES</h6></li>
                      <li v-for="(site, index) in sites" :key="index + 'sites'"><a href="#">{{site}}</a></li>
                  </ul>
              </div>
              <div class="logo-footer">
                  <img src="../assets/img/dc-logo-bg.png" alt="dc-logo">
              </div>
          </div>
      </div>
      <div class="bottom">
          <div class="contenitore">
              <div class="call-to">
              <button> <a href="#">SIGN-UP NOW!</a> </button>
              </div>
              <div class="social">
                  <ul class="social-ul">
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
    name: 'Footer',
    data(){
        return{
            links: [
                'Terms Of Use',
                'Privacy policy',
                'Ad Choices',
                'Advertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshops',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ],
            sites:[
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'Dc Power Visa'
            ]
            

    }
        
    }

}
</script>

<style lang="scss">
@import './src/assets/style/mixins.scss';
footer{
    height: 455px;
    .top{
        height: 70%;
        background-image: url("../assets/img/footer-bg.jpg");
        .contenitore{
            @include center(between);
            height: 100%;
            overflow: hidden;
            .dclist{
                @include center(sinistra);
                align-items: flex-start;
                padding-top: 30px;
                width: 50%;
                height: 100%;
                ul{
                    padding: 0;
                    color: white;
                    margin-right: 30px;
                    li{
                        line-height: 14px;
                        a{
                        color: #6C756E;
                        font-size: 10px;
                        }
                        h6{
                            margin-bottom: 10px;
                        }
                    }
                    .shop{
                        margin-top: 20px;
                    } 
                }
            }
            .logo-footer{
                @include center(destra);
                width: 50%;
                img{
                    width: 90%;
                }
            }
        }
    }
    .bottom{
        height: 30%;
        background-color: #303030;
        @include center();
        .contenitore{
            @include center(between);
            .social{                
                .social-ul{
                    @include center();
                    li{
                        display:inline-block;
                        margin-left: 15px;
                        color: #0088FF;
                        font-size: 25px;  
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