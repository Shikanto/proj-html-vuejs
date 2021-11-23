<template>
    <div class="container">
        <div class="text-center">
            <div class="subtitle">
                LOCATIONS
            </div>
            <h3 class="spacing-title">Visit Our Bakeries</h3>
        </div>
        <div class="d-flex">
            <LocationCard
            v-for="(location, i) in locationList"
            :key="i" :infoLocation="location"
            :index="i">
            ></LocationCard>
        </div>
    </div>
</template>
<script>
import LocationCard from "./LocationCard.vue";

export default {
    name:"Section5",
    components:{
        LocationCard,
    },
    data() {
        return {
            locationList:[
                 {
                    nameLocation: "New York",
                    imgUrl: "new-york-bk-800x530.jpg",
                    numberPhone:"1.800.458.556",
                    timeAm: "9:00",
                    timePm: "6:00",
                    bgColor: "bg-newyork",
                },
                {
                    nameLocation: "London",
                    imgUrl: "london-bk-800x530.jpg",
                    numberPhone:"1.800.458.556",
                    timeAm: "9:00",
                    timePm: "6:00",
                    bgColor: "bg-london",
                }
            ]
        }
    },
}
</script>
<style lang="scss">
    
</style>