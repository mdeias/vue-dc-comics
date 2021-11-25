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
                      <li v-for="(link, index) in links" :key="index">
                          <a :class="{active: link.attivo}" href="#">{{link.text}}</a>
                          </li>
                  </ul>
              </nav>
          </div>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data(){
        return{
            links: [
                {
                    text: 'CHARACTERS',
                    attivo: false
                },
                {
                    text: 'COMICS',
                    attivo: true
                },
                {
                    text: 'MOVIE',
                    attivo: false
                },
                {
                    text: 'TV',
                    attivo: false
                },
                {
                    text: 'GAMES',
                    attivo: false
                },
                {
                    text: 'COLLECTIBLES',
                    attivo: false
                },
                {
                    text: 'VIDEOS',
                    attivo: false
                },
                {
                    text: 'FANS',
                    attivo: false
                },
                {
                    text: 'NEWS',
                    attivo: false
                },
                {
                    text: 'SHOP',
                    attivo: false
                }
            ]
        }
    },
    
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
                    font-size: 11px;
                    a{
                        color: black; 
                        &:hover,
                        &.active{
                            color: #0081FA;
                            padding-bottom: 38px;
                            border-bottom: 4px solid #0081FA;
                        }
                    
                    }
                }
            }
        }
    }
}


</style>