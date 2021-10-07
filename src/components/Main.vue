<template>
  <div id="container-main">
    <TheCompany />
    <ExcellenceInServices />
    <ProcessManagement />
    
  </div>
  <!-- Sezione The Company -->

</template>

<script>
import TheCompany from './TheCompany.vue'
import ExcellenceInServices from './ExcellenceInServices.vue'
import ProcessManagement from './ProcessManagement.vue'

export default {
name: 'Main',
components: {
  TheCompany,
  ExcellenceInServices,
  ProcessManagement,
}
}
</script>

<style scoped lang="scss">

</style>