<template>
  <header class="container-fluid">
   <!-- Sezione header -->
   <HeaderContact />
      <div class="row justify-content-center align-items-center p-4">
        <img class="col-1 me-2" src="../img/nexgen-logo.svg" alt="">
        <NavElement class="col-1 text-center" v-for="(element, index) in navElement" :key="index" :title="element.text" />
        <button class="btn-primary col-2">GET IN TOUCH</button>
      </div>

    <!-- Sezione Jumbotron -->
    <div class="row justify-content-end" id="container-insurance-consulting">
      <div class="col-6">
        <p class="col-12">FUSION e ACQUISITIONS</p>
        <h1 class="col-5 mb-3">Insurance Consulting</h1>
        <div class="row">
          <input class="col-5 m-1 p-2" type="text" placeholder="Name">
          <input class="col-5 m-1 p-2" type="text" placeholder="Email">
          <input class="col-5 m-1 p-2" type="text" placeholder="Phone">
          <input class="col-5 m-1 p-2" type="text" placeholder="More Info">

          <button class="col-3 my-button colored-btn mt-3 me-3">GET IN TOUCH</button>
          <button class="col-3 my-button white-btn mt-3">READ MORE</button>
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
}

#container-insurance-consulting{
  padding: 130px;
}

p{
  color: $primaryColor;
}

h1{
  font-size: 4em;
  font-weight: 600;
}

input{
  background-color: lightgray;
  border-radius: 5px;
  border: none;
}





</style>