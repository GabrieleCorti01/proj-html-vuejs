<template>
  <div class="container-fluid" id="services-container">
      <div class="row justify-content-center">
        <div class="col-7 mt-5">
            <p class="upper-title">OUR BUSINESS AREAS</p>
            <span class="me-4">Excellence in</span> <span class="bg-text">Services</span>
            <p class="mt-3 subtitle-main">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum sapiente quae atque totam repudiandae, natus a esse quaerat asperiores culpa nisi voluptas quidem aperiam aut, reiciendis voluptatibus. Quos, nemo assumenda. asperiores culpa nisi voluptas quidem aperiam aut, reiciendis voluptatibus. Quos, nemo assumenda.</p>
        </div>

        <div class="col-2">
            <button id="see-all-btn" class="my-button colored-btn">SEE ALL</button>
        </div>

        <div class="row justify-content-center mb-5">
            <ServicesElement id="container-elemento" class="col-3 m-4" v-for="(element, index) in excellenceServices" :key="index" :title="element.title" :text="element.text"/>
        </div>
        
        
        
      </div>
      
  </div>
</template>

<script>
import ServicesElement from './ServicesElement.vue'
import excellenceServices from '../data/excellenceInServices'

export default {
    name: 'ExcellenceInServices',
    components: {
      ServicesElement
    },
    data: function (){
      return {
        excellenceServices,
      }
    }

}
</script>


<style lang="scss" scoped>
@import "../style/variable.scss";

span{
  font-size: 2.8em;
  font-weight: 700;
}

#services-container{
background-color: $thirdColor;
}

#container-elemento{
  background-color: white;
  border-radius: 10px;
}

#see-all-btn{
  margin-top: 170px;
  margin-left: 120px;
  padding: 10px 25px;
}

</style>