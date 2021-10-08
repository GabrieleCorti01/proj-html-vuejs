<template>
  <div class="p-5">
    <!-- Icona statica -->
      <div class="d-flex justify-content-end">
          <i class="fas fa-arrow-right"></i>
      </div>
      
    <!-- Elementi dinamici -->
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
@import "../style/variable.scss";

#title{
    font-size: 1.6em;
}

#text{
    font-size: 0.8em;
    color: grey;
    font-weight: 300;
}

i{
    font-size: 2em;
    color: $primaryColor;
}

</style>