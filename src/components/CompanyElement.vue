<template>
  <div>
      <h5 class="fw-bold mb-4"><i class="fas fa-award me-2"></i>{{ title }}</h5>
      <p class="subtitle-main">{{ text }}</p>
  </div>
</template>

<script>
export default {
name: 'CompanyElement',
props: ["title", "text", "icon"]
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";


i{
  color: $primaryColor;
}


</style>