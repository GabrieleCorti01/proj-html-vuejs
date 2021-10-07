<template>
  <div class="container-fluid">
    <div class="row justify-content-center mt-5">
        <div class="col-4 mt-5">
            <p class="upper-title">OUR EDITORIAL CONTENT</p>
            <span>Latest</span><span class="bg-text ms-3">News</span>
            <p class="subtitle-main mt-3">Every week we publish content about what is the best in the business world.</p>
        </div>

        <div class="col-2">
            <button class="my-button colored-btn">SEE ALL</button>
        </div>
    </div>

    
        <NewsElement />
    
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

button{
    margin-top: 100px;
}

</style>