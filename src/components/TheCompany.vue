<template>
  <div class="container-fluid">
      <div class="row">
          <div class="col-4">
              <p>ABOUT THE NETWORK</p>
              <h2>The Company</h2>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, ad eligendi sint ipsum iure, voluptates numquam doloribus placeat ducimus velit quasi pariatur.</p>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, ad eligendi sint ipsum iure, voluptates numquam doloribus placeat</p>
          </div>

          <div class="col-4">
              <CompanyElement />
          </div>
      </div>
  </div>
</template>

<script>
import CompanyElement from './CompanyElement.vue'

export default {
name: 'TheCompany',
components: {
    CompanyElement,
}
}
</script>

<style lang="scss" scoped>

h2{
    font-size: 2.8em;
    font-weight: 600;
}

</style>