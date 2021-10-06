<template>
  <div id="app">
    <Contact />
    <Header />
    <Main />
    <Footer />

  </div>
</template>

<script>
import Contact from './components/Contact.vue'
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'



export default {
  name: 'App',
  components: {
    Contact,
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import "./style/variable.scss";


*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Ubuntu';
}



</style>
