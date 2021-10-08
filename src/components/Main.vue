<template>
  <div id="container-main">
    <TheCompany />
    <ExcellenceInServices />
    <ProcessManagement />
    <TeamOfExperts />
    <LatestNews />
    <KnowFirst />
    
    
  </div>
</template>

<script>
import TheCompany from './TheCompany.vue'
import ExcellenceInServices from './ExcellenceInServices.vue'
import ProcessManagement from './ProcessManagement.vue'
import TeamOfExperts from './TeamOfExperts.vue'
import LatestNews from './LatestNews.vue'
import KnowFirst from './KnowFisrt.vue'

export default {
name: 'Main',
components: {
  TheCompany,
  ExcellenceInServices,
  ProcessManagement,
  TeamOfExperts,
  LatestNews,
  KnowFirst
}
}
</script>

<style scoped lang="scss">

</style>