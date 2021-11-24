<template>
  <div>
    
   <Header/>
   <Main/>
   <Merch/>
   <Footer/>

  </div>
</template>

<script>
import Header from '../src/components/Header.vue';
import Main from '../src/components/Main.vue';
import Merch from '../src/components/Merch.vue';
import Footer from '../src/components/Footer.vue';

export default {
  name: 'App',

  components: {
    Header,
    Main,
    Merch,
    Footer
  }
}
</script>

<style lang="scss">

</style>
