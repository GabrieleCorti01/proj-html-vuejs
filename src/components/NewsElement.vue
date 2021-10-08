<template>
    <div class="row justify-content-center text-center p-4">
    <!-- Sezione vari elementi statici news -->
        <div class="element-box box-1 col-4 m-2 p-3 align-items-end d-flex">
            <p>Increasing creativity is possible for everyone</p>
        </div>
    <!-- Sezione vari elementi statici news -->
        <div class="element-box box-2 col-4 m-2 p-3 align-items-end d-flex">
            <p>Because market research is part of the business plan</p>
        </div>
    <!-- Sezione vari elementi statici news -->   
        <div class="element-box box-3 col-4 m-2 p-3 align-items-end d-flex">
            <p>Working from home is now a trend</p>
        </div>
    </div>
</template>

<script>
export default {
name: 'NewsElement',
}
</script>

<style lang="scss" scoped>

.element-box{
    width: 300px;
    height: 300px;
    background-size: contain;
    border-radius: 10px;
    color: white;
}

.box-1{
    background-image: url("../img/news-1.jpg");
}

.box-2{
background-image: url("../img/news-2.jpg");
}

.box-3{
background-image: url("../img/news-3.jpg");
}

p{
    font-size: 1.3em;
}

</style>