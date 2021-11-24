<template>
  <header>
      <div class="contenitore">
          <div class="logo">
          <a href="#">
              <img src="../assets/img/dc-logo.png" alt="">
          </a>
          </div>
          <div class="nav-bar">
              <nav>
                  <ul>
                      <li><a href="#">CHARACTERS</a></li>
                      <li><a href="#">COMICS</a></li>
                      <li><a href="#">MOVIE</a></li>
                      <li><a href="#">TV</a></li>
                      <li><a href="#">GAMES</a></li>
                      <li><a href="#">COLLECTIBLES</a></li>
                      <li><a href="#">VIDEOS</a></li>
                      <li><a href="#">FANS</a></li>
                      <li><a href="#">NEWS</a></li>
                      <li><a href="#">SHOP</a></li>
                  </ul>
              </nav>
          </div>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss">
@import './src/assets/style/mixins.scss';

header{
    height: 100px;
    @include center();
    .contenitore{
        @include center(between);
        .logo{
         width: 70px;
        }
        .nav-bar{
            @include center(align);
            nav{  
                ul li{
                   
                    display: inline-block;
                    margin-left: 10px;
                    color: black;
                    font-size: 12px;
                    a{
                        color: black; 
                        &:hover{
                            color: blue;
                        }
                    
                    }
                }
            }
        }
    }
}


</style>