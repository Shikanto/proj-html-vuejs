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
             v-for="(product, i) in getListProduct().slice(0, 2)"
             :key="i" 
             :infoProduct="product">
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
    data() {
        return {
            listProduct:[],
        }
    },
    components:{
        ProductsSlider,
    },
    props:{
        productsShop: Array,
    },
    methods: {
        getListProduct(){
            this.listProduct = this.productsShop
            console.log(this.productsShop)
            console.log(this.listProduct)
            return this.listProduct;
        }
    },
}
</script>
<style lang="scss">

</style>