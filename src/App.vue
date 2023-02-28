<script>
//import
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Main from './components/Main.vue';
import Comics from '../src/_comics';
//export
export default {
  components: {
    Header,
    Footer,
    Main,
    Comics
  },

  data (){
    return{
      Comics,
    }
  }

}
</script>

<template>
  <!-- stampo su html -->
    <Header />
    <Main :comicsList="Comics" />
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

.flex{
  display: flex;
}

.wrap{
  flex-wrap: wrap;
}


img{
  max-width: 100%;
}

ul {
  list-style-type: none;
}

ul li{
  margin: 0.5rem;
}

ul li a {
  color: inherit;
  text-decoration: none;
}


</style>
