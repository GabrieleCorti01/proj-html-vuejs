<template>
  <div class="container-link me-4">
    <!-- Lista dinamica non ordinata -->
      <ul>
          <h5>{{ title }}</h5>
          <li><a href="#"><i class="fas fa-chevron-right me-2 mt-2"></i>{{ link1 }}</a></li> 
          <li><a href="#"><i class="fas fa-chevron-right me-2"></i>{{ link2 }}</a></li>
          <li><a href="#"><i class="fas fa-chevron-right me-2"></i>{{ link3 }}</a></li>
          <li><a href="#"><i class="fas fa-chevron-right me-2"></i>{{ link4 }}</a></li>
          <li><a href="#"><i class="fas fa-chevron-right me-2"></i>{{ link5 }}</a></li>
          <li><a href="#"><i class="fas fa-chevron-right me-2"></i>{{ link6 }}</a></li>
      </ul>
  </div>
</template>

<script>
export default {
name: 'FooterLink',
props :[ "title", "link1", "link2", "link3", "link4", "link5", "link6", ]
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

.container-link{
    background-color: #242427;
    width: 220px;
    border-radius: 10px;
    padding: 40px 0;
    h5{
        font-weight: 700;
    }
    ul{
        list-style: none;
    }
    li{
        font-weight: 300;
        a{
            text-decoration: none;
            color: lightgray;
        } a:hover{
            color: $primaryColor;
        }
    }
}

</style>