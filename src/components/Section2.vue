<template>
    <div class="container">
        <div class="text-center">
            <div class="subtitle">CORPORATE & WEDDINGS</div>
            <h3 class="spacing-title">Baking Special Moment</h3>
        </div>
        <div class="container-special-moments d-flex">
           <SpecialMoments 
           v-for="(moment, i) in SpecialMoment"
             :key="i" :infoMoment="moment">
           ></SpecialMoments>
        </div>
    </div>
</template>
<script>
import SpecialMoments from "./SpecialMoments.vue";

export default {
    name:"Section2",
    components:{
        SpecialMoments,
    },
    data() {
        return {
            SpecialMoment: [
                {
                    imgShow:"corporate-bg.jpg",
                    imgHover:"corporate-hover-bg.jpg",
                    nameEvent:"international bakery",
                    typeEvent:"Corporate Events",
                },
                {
                    imgShow:"wedding-bg.jpg",
                    imgHover:"wedding-hover-bg.jpg",
                    nameEvent:"private dining hall",
                    typeEvent:"Weddings & Parties",
                },

            ]
        }
    },
}
</script>
<style lang="scss">
    
</style>