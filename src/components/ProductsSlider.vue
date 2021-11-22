<template>
    <div class="cardProducts">
        <img  class="imgProduct"
        :src="require(`../assets/${infoProduct.urlImg}${infoProduct.sizeImgBig}`)" 
        :alt="infoProduct.nameProduct">
        <div class="overlay">
            <div class="nameProduct"><strong>{{infoProduct.nameProduct}}</strong></div>
            <div class="typeProduct">{{infoProduct.type}}</div>
            <div class="priceProduct">${{infoProduct.lowPrice}}  ${{infoProduct.topPrice}}</div>
        </div>
    </div>
</template>
<script>
export default {
    name:"ProductsSlider",
    props:{
        infoProduct: Object,
    }
}
</script>
<style lang="scss">

</style>