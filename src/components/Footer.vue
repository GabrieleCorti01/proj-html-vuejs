<template>
  <div class="container-fluid">
    <div class="row p-5 justify-content-center">
  <!-- Sezione statica contatti sinistra -->
      <div class="col-2">
        <img src="../img/nexgen-logo.svg" alt="logo azinda footer">
        <p class="subtitle-main mt-4">A Functional HTML Template for Corporate e Business.</p>
        <p class="subtitle-main"><i class="fas fa-phone me-2"></i>+1 (305) 1234-5678</p>
        <p class="subtitle-main"><i class="fas fa-envelope me-2"></i>hello@example.com</p>
        <p class="subtitle-main"><i class="fas fa-map-marker-alt me-2"></i>Main Avenue,987</p>
        <button class="my-button custom-btn mt-2">GET IN TOUCH</button>
      </div>
  <!-- Sezione dinamica links destra -->
      <FooterLink class="col-2" v-for="(element, index) in footerElement" :key="index" :title="element.title" :link1="element.link1" :link2="element.link2" :link3="element.link3" :link4="element.link4" :link5="element.link5" :link6="element.link6"/>
    </div>
  <!-- Sezione underfooter con privacy  -->
    <FooterPrivacy />
  </div>
</template>

<script>
import FooterLink from './FooterLink.vue'
import footerElement from '../data/footerElement'
import FooterPrivacy from './FooterPrivacy.vue'

export default {
name: 'Footer',
components: {
  FooterLink,
  FooterPrivacy
},
data: function(){
  return {
    footerElement
  }
}
}
</script>

<style scoped lang="scss">
@import "../style/variable.scss";

.container-fluid{
  background-color: $secondaryColor;
  color: white;
  
  img{
    width: 150px;
  }

  .custom-btn{
    background-color: $secondaryColor;
    border: 1px solid $primaryColor;
    color: white;
  }
}

</style>