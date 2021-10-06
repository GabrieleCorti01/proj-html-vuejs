<template>
  <ul>
      <li>{{ title }}</li>
  </ul>
</template>

<script>
export default {
name: 'NavElement',
props: ["title"]
}

</script>

<style lang="scss" scoped>
ul{
    list-style: none;
}
</style>