<template>
  <header class="container-fluid">
  <!-- Sezione statica Header contatti -->
   <HeaderContact />

  <!-- Sezione principale Header -->
  <div class="row justify-content-center p-3 align-items-end">
    <img src="../img/nexgen-logo.svg" class="col-1" alt="">

  <!-- Sezione dinamica elenco non numerato nav -->
    <NavElement class="col-1" v-for="(element, index) in navElement" :key="index" :title="element.text" />

  <!-- Bottone Nav -->
    <button class="col-1 my-button colored-btn btn-hover-colored">GET IN TOUCH</button>
    </div>

  <!-- Sezione Jumbotron -->
    <div class="row justify-content-end" id="container-insurance-consulting">
      
      <div class="col-6">

        <p class="col-12">FUSION e ACQUISITIONS</p>

        <h1 class="col-5 mb-3">Insurance Consulting</h1>

  <!-- Sezione input di testo statici -->
        <div class="row">
          <input class="col-5 m-1 p-2" type="text" placeholder="Name">

          <input class="col-5 m-1 p-2" type="text" placeholder="Email">

          <input class="col-5 m-1 p-2" type="text" placeholder="Phone">

          <input class="col-5 m-1 p-2" type="text" placeholder="More Info">
  <!-- Sezione bottoni con hover statici -->
          <button class="col-3 my-button colored-btn mt-3 me-3 btn-hover-colored">GET IN TOUCH</button>
          <button class="col-3 my-button white-btn mt-3 btn-hover-white">READ MORE</button>
        </div>
      </div>
    </div>



  </header>
</template>

<script>
import NavElement from './NavElement.vue'
import navElement from '../data/navElement'
import HeaderContact from './HeaderContact.vue'

export default {
name: 'Header',
components: {
  NavElement,
  HeaderContact
},
data: function (){
        return {
            navElement,
        }
    }
}
</script>

<style scoped lang="scss">
@import "../style/variable.scss";

header{
  height: 800px;
  background-image: url("../img/bg-6.jpg");
  background-size: cover;
  background-position: top;
}

#container-insurance-consulting{
  padding: 130px;
}

img{
  margin-right: 250px;
}

p{
  color: $primaryColor;
}

h1{
  font-size: 4em;
  font-weight: 700;
}

input{
  background-color: lightgray;
  border-radius: 5px;
  border: none;
}





</style>