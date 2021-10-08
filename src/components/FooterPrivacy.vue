<template>
  <div class="row justify-content-center text-center">
      <div class="col-4">
          <p>Enjoy the low price. We are tracking any intention of piracy.</p>
      </div>

      <div class="col-4">
          <p><i class="far fa-copyright"></i> 2020 NEXGEN is Proudly Powered by <span>Codings</span>.</p>
      </div>
  </div>

</template>

<script>
export default {
name: 'FooterPrivacy',
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

.row{
    background-color: black;
    padding: 30px 0 10px 0;
    p{
        font-size: 0.7em;
        font-weight: 300;
    }
    span{
        color: $primaryColor;
    }
}

</style>