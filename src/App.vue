<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'



export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import "./style/variable.scss";
@import '~@fortawesome/fontawesome-free/css/all.css';


*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Ubuntu';
}

a{
  text-decoration: none;
}



</style>
