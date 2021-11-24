<template>
  <div class="container-img-special-moments">
    <img :src="require(`../assets/${infoMoment.imgShow}`)" alt="" />
    <div class="overlay">
        <img class="absolute" :src="require(`../assets/${infoMoment.imgHover}`)" alt="">
        <div class="text-center absolute indexPlus">
            <div class="subtitle-hover">{{infoMoment.nameEvent.toUpperCase()}}</div>
            <h2>{{infoMoment.typeEvent}}</h2>
            <div>
                <button class="btn btn-purple">Explore more</button>
            </div>
        </div>
    </div>
    <div class="overlay"></div>
  </div>
</template>
<script>
export default {
  name: "SpecialMoments",
  props:{
      infoMoment: Object,
  }
};
</script>
<style lang="scss">

</style>