<template>
    <section class="container d-flex">
        <div class="ourProducts">
            <div class="subtitle">
                OUR PRODUCTS
            </div>
            <div class="spacing-title">
                <h3>All our delectable pastries are
                    backed fresh in our Kitchen very
                    morning, anda are made with all-
                    natural, all organic ingredients.
                </h3>
            </div>
            <div>
                <button class="btn btn-purple">Start Shopping</button>
            </div>
        </div>
        <div class="sliderProducts d-flex gap">
            <ProductsSlider
             v-for="(product, i) in productsShop"
             :key="i" :infoProduct="product">
            </ProductsSlider>
            <div class="arrow arrow-left">
                <i class="fa fa-chevron-left" aria-hidden="true"></i>
            </div>
            <div class="arrow arrow-right">
                <i class="fa fa-chevron-right" aria-hidden="true"></i>
        </div>
        </div>
    </section>
</template>
<script>
import ProductsSlider from "./ProductsSlider.vue"


export default {
    name:"Section1",
    components:{
        ProductsSlider,
    },
    data() {
        return {
            productsShop:[
                {
                    nameProduct: "Choco Chip Cookies",
                    urlImg: "choco-chip-cookies-",
                    sizeImgBig: "700x893.jpg",
                    sizeImgSmall: "200x255.jpg",
                    type: "Cookies, Pastries",
                    lowPrice: "19.00",
                    topPrice: "39.00",
                },
                {
                    nameProduct: "Strawberry Jam Cookies",
                    urlImg: "strawberry-jam-cookies-",
                    sizeImgBig: "700x893.jpg",
                    sizeImgSmall: "200x255.jpg",
                    type: "Cookies, Pastries",
                    lowPrice: "24.00",
                    topPrice: "62.00",
                },
                /* {
                    nameProduct: "Strawberry Donut",
                    urlImg: "strawberry-jam-cookies-",
                    sizeImgBig: "400x510.jpg",
                    sizeImgSmall: "200x255.jpg",
                    type: "Donuts, Pastries",
                    lowPrice: "24.00",
                    topPrice: "48.00",
                },
                {
                    nameProduct: "Perfect MAcarons",
                    urlImg: "perfect-macarons-",
                    sizeImgBig: "400x510.jpg",
                    sizeImgSmall: "200x255.jpg",
                    type: "macarons, Pastries",
                    lowPrice: "32.00",
                    topPrice: "56.00",
                }, */
            ] 
        }
    },
}
</script>
<style lang="scss">

</style>