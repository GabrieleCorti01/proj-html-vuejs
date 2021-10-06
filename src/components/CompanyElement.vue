<template>
  <div >
      <h5 class="fw-bold mb-4">{{ title }}</h5>
      <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
name: 'CompanyElement',
props: ["title", "text"]
}
</script>

<style lang="scss" scoped>
p{
    color: lightgrey;
    font-size: 0.8em;
}


</style>