<template>
  <div id="app">
    <Header> </Header>
    <main>
      <Section1
        :productsShop="shop"
        class="spacing-section"
      ></Section1>
      <Section2 class="spacing-section"></Section2>
      <Section3 
      :productsShop="shop"
      class="spacing-section">
      </Section3>
      <Section4 class="spacing-section"></Section4>
      <Section5 class="spacing-section"></Section5>
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Section1 from "./components/Section1.vue";
import Section2 from "./components/Section2.vue";
import Section3 from "./components/Section3.vue";
import Section4 from "./components/Section4.vue";
import Section5 from "./components/Section5.vue";

export default {
  name: "App",
  components: {
    Header,
    Section1,
    Section2,
    Section3,
    Section4,
    Section5,
  },
  data() {
    return {
      shop: [
        {
          nameProduct: "Choco Chip Cookies",
          urlImg: "choco-chip-cookies-",
          sizeImgBig: "700x893.jpg",
          sizeImgSmall: "400x510.jpg",
          type: "Cookies, Pastries",
          lowPrice: "19.00",
          topPrice: "39.00",
        },
        {
          nameProduct: "Strawberry Jam Cookies",
          urlImg: "strawberry-jam-cookies-",
          sizeImgBig: "700x893.jpg",
          sizeImgSmall: "400x510.jpg",
          type: "Cookies, Pastries",
          lowPrice: "24.00",
          topPrice: "62.00",
        },
        {
          nameProduct: "Strawberry Donut",
          urlImg: "strawberry-donut-",
          sizeImgBig: "400x510.jpg",
          sizeImgSmall: "400x510.jpg",
          lowPrice: "24.00",
          topPrice: "42.00",
        },
        {
          nameProduct: "Perfect MAcarons",
          urlImg: "perfect-macarons-",
          sizeImgBig: "400x510.jpg",
          sizeImgSmall: "400x510.jpg",
          lowPrice: "18.00",
          topPrice: "52.00",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "style/app.scss";
</style>
