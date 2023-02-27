<script>
//import
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Main from './components/Main.vue';

//export
export default {
  components: {
    Header,
    Footer,
    Main
  }

}
</script>

<template>
  <!-- stampo su html -->
    <Header />
    <Main />
    <Footer />
</template>

<style lengs="scss">
/* regole base  */
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.container{
  max-width: 1200px;
  margin: auto;
}

img{
  max-width: 100%;
}

ul {
  list-style-type: none;

  li{
    margin: 0.5rem;
  
    a{
      color: inherit;
      text-decoration: none;
    }
  }
}


</style>
