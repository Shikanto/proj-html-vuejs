<template>
    <div class="cardProducts">
        <img  class="imgProduct"
        :src="require(`../assets/${infoProduct.urlImg}${infoProduct.sizeImgBig}`)" 
        :alt="infoProduct.nameProduct">
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