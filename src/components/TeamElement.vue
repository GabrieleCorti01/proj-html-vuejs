<template>
  <div class="row">
      <div class="col-5">
          <img :src="source" alt="">
      </div>

      <div class="col-7">
          <p id="title">{{ name }}</p>
          <p class="subtitle-main" id="subtitle">{{ subtitle }}</p>
          <div id="container-icons">
              <i class="fab fa-facebook-f"></i>
              <i class="fab fa-twitter"></i>
              <i class="fab fa-linkedin-in"></i>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'TeamElement',
    props: ["name", "subtitle", "source"]
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

img{
    width: 100%;
}

#container-icons{
    i{
        font-size: 0.6em;
        margin-right: 10px;
        color: $primaryColor;
        background-color: rgb(4, 131, 131, 0.15);
        padding: 10px;
        border-radius: 3000px;
    }
}

#title{
    font-size: 1.1em;
    font-weight: 700;
}

#subtitle{
    font-size: 0.7em;
}

</style>