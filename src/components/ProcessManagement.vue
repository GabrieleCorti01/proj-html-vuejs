<template>
  <div class="container-fluid">
      <div class="row justify-content-center text-center">
    <!-- Parte di intestazione statica -->
          <div class="col-5 mt-5">
              <p class="upper-title mt-5">HOW IT WORKS IN PRACTICE</p>
              <span class="bg-text me-2">Process</span><span>Management</span>
              <p class="subtitle-main mt-4">We work with innovative methodologies to ensure that the entire reformatting process is done from start to finish as planned</p>
          </div>
    <!-- Parte dei contenuti dinamica -->
          <div class="row justify-content-center mb-5">
              <ProcessElement class="col-2 mb-4" v-for="(element, index) in managementElement" :key="index" :number="element.number" :title="element.title" :text="element.text"/>
          </div>
      </div>
  </div>
</template>

<script>
import ProcessElement from './ProcessElement.vue';
import managementElement from '../data/managementElement'

export default {
name: 'ProcessManagement',
components: {
    ProcessElement
},
data: function (){
      return {
        managementElement,
      }
    }
}
</script>

<style lang="scss" scoped>

span{
    font-size: 2.8em;
    font-weight: 700;
}

</style>