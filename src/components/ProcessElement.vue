<template>
  <!-- Sezione elementi dinamici -->
  <div>
    <p id="number-style" class="justify-content-center">{{ number }}</p>
    <p id="title">{{ title }}</p>
    <p class="subtitle-main">{{ text }}</p>
  </div>
</template>

<script>
export default {
name: 'ProcessElement',
 props: ["number", "title", "text"]
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

#number-style{
    color: $primaryColor;
}

#title{
    font-size: 1.2em;
    font-weight: 700;
}

</style>