<template>
  <div id="app">
    <header>
      <Navbar />
    </header>
    <v-content>
     <Carousel/>
    </v-content>
    <br>

     <v-content>
    <Products/>
    </v-content>
    <br>
    
    <Footer/>
  </div>
</template>

<script>
    
     
import Navbar from './components/Navbar';
import Carousel  from './components/Carousel';
import Products  from './components/Products';
import Footer  from './components/Footer';
export default {
  name: 'app',
  components: {
    Navbar,
    Carousel,
    Products,
    Footer
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: 'montserrat', sans-serif;
}
header {
  width: 100vw;
  background-color: #222;
  padding: 15px;
}
</style>