<template>
    <div class="container">
        <div class="container-shop d-flex">
            <div class="container-shop-text text-center">
                <h3>Find a freshly baked product perfect for you</h3>
                <div class="spacing-title">
                    Integer a nibh vitae ex porttitor rutrum et ut
                    velit. Etiam ac felis at leo feugiat placerat. Sed
                    ac nulla id orci tempor convallis sed.
                </div>
                <div>
                    <button class="btn btn-purple">Shop All Products</button>
                </div>

            </div>
            <div class="slider-shop d-flex">
                <SliderShop
                v-for="(product, i) in getListProduct()"
                :key="i" 
                :infoProduct="product">
                ></SliderShop>
                <div class="arrow arrow-left">
                    <i class="fa fa-chevron-left" aria-hidden="true"></i>
                </div>
                <div class="arrow arrow-right">
                    <i class="fa fa-chevron-right" aria-hidden="true"></i>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import SliderShop from "./SliderShop.vue"


export default {
   name:"Section3",
   data() {
       return {
           listProduct:[],
       }
   },
   components: {
       SliderShop,
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