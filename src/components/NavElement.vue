<template>
    <div class="col-1">
      <ul>
        <li><a href="#" >{{ title }}</a></li>
      </ul>
    </div>

</template>

<script>
export default {
name: 'NavElement',
props: ["title"]
}

</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

ul{
    list-style: none;
    a{
      color: $secondaryColor;
    } a:hover{
      color: $primaryColor;
    }
}
</style>