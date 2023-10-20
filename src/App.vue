<template>
  <div id="App" class="bg-color-#EFEFEF">
    <Navbar/>
    <Body/>
    <Footer/>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue' ;
import Footer from './components/Footer.vue';
import Body from './components/bodyLanding.vue';
export default {
  name: 'App',
  components: {
    Navbar,
    Body,
    Footer,

  }
}
</script>

<!-- <style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
 -->