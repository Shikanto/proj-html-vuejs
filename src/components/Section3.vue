<template>
    <div class="container">
        <div class="container-shop d-flex">
            <div class="container-shop-text text-center">
                <h3>Find a freshly baked product perfect for you</h3>
                <div class="spacing-title text-gray ">
                    Integer a nibh vitae ex porttitor rutrum et ut
                    velit. Etiam ac felis at leo feugiat placerat. Sed
                    ac nulla id orci tempor convallis sed.
                </div>
                <div>
                    <button class="btn btn-purple">Shop All Products</button>
                </div>

            </div>
            <div class="slider-shop d-flex">
                <SliderShop class="hide"
                :class="i >= minRange && i <= maxRange ? 'active' : 'back-img'"
                v-for="(product, i) in getListProduct()"
                :key="i" 
                :infoProduct="product">
                ></SliderShop>
                <div @click="goLeft" class="arrow arrow-left">
                    <i class="fa fa-chevron-left" aria-hidden="true"></i>
                </div>
                <div @click="goRight" class="arrow arrow-right">
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
           minRange: 0.,
           maxRange:3,
           currentIndex: 0,
           classActive:"",
           
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
            //console.log(this.productsShop)
            //console.log(this.listProduct)
            return this.listProduct;
        },
        goRight(){
            this.minRange ++;
            this.maxRange ++;
            if(this.maxRange > this.getListProduct().length -1) {
                this.maxRange = 3;     
                this.minRange = 0;           
            } 
        },
        goLeft(){
            this.minRange --;
            this.maxRange --;
            if (this.minRange < 0) {
                this.minRange = this.productsShop.length -4;
                this.maxRange = this.productsShop.length -1;
            } 
        },
       /*  checkIndex(index){

            if(index >= this.minRange && index <= this.maxRange) {
                this.classActive = 'active'
            }  else if (index <= this.minRange || index >= this.maxRange)
                this.classActive = 'active' 
            else {
                this.classActive = 'back-img'
            }

            return this.classActive
        } */
    },
}
</script>
<style lang="scss">
    
</style>