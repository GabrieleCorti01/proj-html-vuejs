<template>
  <div class="container-fluid">
      <div class="row justify-content-center ">
          <div class="col-3 me-5 my-container-box">
              <p id="upper-title">ABOUT THE NETWORK</p>
              <span class="me-1" id="back-text">The</span> <span class>Company</span>
              <p class="mt-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, ad eligendi sint ipsum iure, voluptates numquam doloribus placeat ducimus velit quasi pariatur.</p>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, ad eligendi sint ipsum iure.</p>
          </div>

          <div class="col-4 ms-5 my-container-box">
              <div class="row">
                  <CompanyElement class="col-5 mb-4" v-for="(element, index) in companyElement" :key="index" :title="element.title" :text="element.text"/>
              </div>
              
          </div>
      </div>
  </div>
</template>

<script>
import CompanyElement from './CompanyElement.vue'
import companyElement from '../data/companyElement'

export default {
name: 'TheCompany',
components: {
    CompanyElement,
    },
    data: function(){
        return {
            companyElement,
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

.container-fluid{
    background-color: $secondaryColor;
    color: white;
}

.my-container-box{
    padding: 100px 0 100px 0;
}

span{
    font-size: 2.8em;
    font-weight: 600;
}

p{
    color: lightgrey;
    font-size: 0.8em;
}

#upper-title{
    font-size: 0.9em;
    color: $primaryColor;
}

#back-text{
    background-color: rgb(4, 131, 131, 0.4);
    padding: 3px 12px;
    border-radius: 5px;
}


</style>