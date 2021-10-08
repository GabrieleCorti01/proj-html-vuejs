<template>
  <section class="row justify-content-center    ">
    <!-- Sezione statica contatti sinistra -->
      <div class="col-4 pt-3">
          <p><i class="fas fa-clock me-2"></i>Open Hours: Mon - Sat - 9:00 - 18:00</p>
      </div>

    <!-- Sezione statica contatti destra -->
      <div class="col-4 pt-3 d-flex">
          <p class="me-4"><i class="fas fa-phone me-2"></i>+1 (305) 1234-5678</p>
          <p class="me-5"><i class="fas fa-envelope me-2"></i>hello@example.com</p>
          <a href="#"><i class="fab fa-facebook-f me-4"></i></a>
          <a href="#"><i class="fab fa-twitter me-4"></i></a>
          <a href="#"><i class="fab fa-linkedin-in"></i></a>
      </div>
  </section>
</template>

<script>
export default {
    name: 'HeaderContact'

}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

.row{
    background-color: $secondaryColor;
    color: lightgray;
    font-weight: 300;
    align-items: center;
    a{
        color: lightgray;
    } a:hover{
        color: $primaryColor;
        font-size: 1.1em;
    }
}

</style>