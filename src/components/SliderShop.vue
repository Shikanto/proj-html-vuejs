<template>
    <div class="shop-card">
        <div class="imgShopCard">
            <img :src="require(`../assets/${infoProduct.urlImg}${infoProduct.sizeImgSmall}`)" 
            :alt="infoProduct.nameProduct">
            <div class="overlay">
                <h5>SELECT OPTIONS / QUICK VIEW</h5>
            </div>
        </div>
        
        <div class="textShopCard text-center">
            <h4>{{infoProduct.nameProduct}}</h4>
            <div class="priceProduct">${{infoProduct.lowPrice}} - ${{infoProduct.topPrice}}</div>
        </div>
    </div>
</template>
<script>
export default {
    name:"SliderShop",
    props:{
        infoProduct: Object,
    }
}
</script>
<style lang="scss">
    
</style>