<template>
  <div class="container-fluid">
    <!-- Sezione contenitrice -->
      <div class="row justify-content-center p-4" id="container-know-first">

    <!-- Colonna elementi statici sinistra -->
        <div class="col-3 container-column me-5 ">
            <p class="upper-title">NEWSLETTER</p>
            <span class="bg-text-white me-2">Know</span><span>First</span>
            <p class="subtitle-main mt-3" id="subtitle-custom">Follow closely and receive content about our company and the news of the current market.</p>
        </div>

    <!-- Colonna elementi statici destra -->
        <div class="col-2 container-column">
            <input class="mb-3 p-2" type="text" placeholder="Name"><br>
            <input class="mb-3 p-2" type="text" placeholder="Email"><br>
            <button class="my-button colored-btn padding-button mb-5 btn-hover-colored">Subscribe</button>
        </div>
      </div>
  </div>
</template>

<script>
export default {
name: 'KnowFirst',
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

#subtitle-custom{
    color: white;
}

.container-column{
    padding: 80px 0 60px 0;
}

.container-fluid{
    background-image: url("../img/bg-1.jpg");
    background-size: cover;
    background-position: 50%;
}

span{
    font-size: 2.8em;
    font-weight: 700;
    color: white;
}

input{
    opacity: 50%;
    width: 350px;
    border-radius: 5px;
    border: none;
}

.padding-button{
    padding: 10px 25px 10px 25px;
}

</style>