<template>
  <div class="container-fluid">
    <!-- Sezione contenitrice -->
    <div class="row justify-content-center mt-5">
    <!-- Sezione colonna statica superiore -->
        <div class="col-4 mt-5">
            <p class="upper-title">OUR EDITORIAL CONTENT</p>
            <span>Latest</span><span class="bg-text ms-3">News</span>
            <p class="subtitle-main mt-3">Every week we publish content about what is the best in the business world.</p>
        </div>

    <!-- Sezione bottone -->
        <div class="col-2">
            <button class="my-button colored-btn btn-hover-colored" id="news-button">SEE ALL</button>
        </div>
    </div>
    <!-- Sezione dinamica news interna solo alla main row -->
        <NewsElement class="mb-5"/>
  </div>
</template>

<script>
import NewsElement from './NewsElement.vue'
import newsElement from '../data/newsElement'

export default {
name: 'LatestNews',
components: {
    NewsElement
},
data: function(){
    return{
        newsElement
    }
}

}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

span{
    font-size: 2.8em;
    font-weight: 700;
}

#news-button{
    margin-top: 150px;
    margin-left: 150px;
}

</style>