<template>
  <div id="container-main">
    <TheCompany />
    <ExcellenceInServices />
  </div>
  <!-- Sezione The Company -->

</template>

<script>
import TheCompany from './TheCompany.vue'
import ExcellenceInServices from './ExcellenceInServices.vue'

export default {
name: 'Main',
components: {
  TheCompany,
  ExcellenceInServices,
}
}
</script>

<style scoped lang="scss">

</style>