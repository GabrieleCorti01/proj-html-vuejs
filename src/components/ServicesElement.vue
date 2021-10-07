<template>
  <div class="p-5">
      <div class="d-flex justify-content-between">
          <span>ic</span> <span>ic</span>
      </div>
      
      <p id="title">{{ title }}</p>
      <p id="text">{{ text }}</p>
  </div>
</template>

<script>
export default {
    name: 'ServicesElement',
    props: ["title", "text"]

}
</script>

<style lang="scss" scoped>

#title{
    font-size: 1.6em;
}

#text{
    font-size: 0.8em;
    color: grey;
    font-weight: 300;
}

</style>