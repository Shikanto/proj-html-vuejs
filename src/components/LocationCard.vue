<template>
  <div class="card-location">
    <div class="img-location">
      <img
        :src="require(`../assets/${infoLocation.imgUrl}`)"
        :alt="infoLocation.nameLocation"
      />
    </div>
    <div class="info-location text-center d-flex" :class="getBgColor()">
      <h3>{{ infoLocation.nameLocation }}</h3>
      <div class="container-info d-flex">
        <div class="width-info">
          <div class="subtitle">CALL US</div>
          <div class="subtitle margin-subtitle">{{ infoLocation.numberPhone }}</div>
        </div>
        <div class="width-info">
          <div class="subtitle">OPEN ALL WEEK</div>
          <div class="subtitle margin-subtitle">
            {{ infoLocation.timeAm }} AM - {{ infoLocation.timePm }} PM
          </div>
        </div>
        <div class="width-info">
          <button class="btn btn-white">View Map</button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "LocationCard",
  props: {
    infoLocation: Object,
    index: Number
  },
  data() {
      return {
          currentIndex: 0,
          bgColorLocation: "",
      }
  },
  methods: {
      getBgColor() {
            this.bgColorLocation = this.infoLocation.bgColor
            return this.bgColorLocation
        }
    }

};
</script>
<style lang="scss">
</style>