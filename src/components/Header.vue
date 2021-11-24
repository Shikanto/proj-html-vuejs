<template>
  <header class="bg-hero">
    <div class="navBar d-flex">
      <div id="logo">
        <img :src="require('../assets/avada-bakery-logo.png')" alt="" />
      </div>
      <ul class="d-flex">
        <NavLinks v-for="(link, i) in linksNavBar" :key="i" :infoLink="link">
        </NavLinks>
        <li>
          <a href="#"><i class="fa fa-shopping-cart" aria-hidden="true"></i></a>
        </li>
      </ul>
    </div>

    <!-- ICONS RIGHT -->

    <div class="demosOnSale d-flex">
      <div class="container-demos d-flex">
        <div class="container-icon-demos d-flex">
          <div class="demos-sale">
            <i class="fa fa-database" aria-hidden="true"></i>
          </div>
          <div class="text-demos">Demos</div>
        </div>
        <div class="container-icon-demos">
          <div class="demos-sale sale-price">
            <div class="dollar">$</div>
            39
          </div>
          <div class="text-demos">On sale</div>
        </div>
      </div>
    </div>

    <!-- HERO -->

    <div class="container">
      <div class="hero">
        <div class="subtitle">FRESH & TASTY BAKERY EVERY DAY</div>
        <div class="spacing-title"><h1>The Perfect Fresh Bread</h1></div>
        <div class="text-hero text-gray">
          Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl
          varius. Aliquam erat volutpat. Nullam quis sagittis nibh ac nulla id
          orci tempor.
        </div>
        <div class="">
          <button class="btn btn-white">Explore our product</button>
        </div>
      </div>
    </div>
  </header>
</template>
<script>
import NavLinks from "./NavLinks.vue";

export default {
  name: "Header",
  components: {
    NavLinks,
  },
  data() {
    return {
      linksNavBar: [
        {
          nameLink: "HOME",
          active: "True",
          href: "#",
        },
        {
          nameLink: "SHOP",
          active: "False",
          href: "#",
        },
        {
          nameLink: "ABOUT",
          active: "False",
          href: "#",
        },
        {
          nameLink: "GALLERY",
          active: "False",
          href: "#",
        },
        {
          nameLink: "LOCATIONS",
          active: "False",
          href: "#",
        },
        {
          nameLink: "JOURNAL",
          active: "False",
          href: "#",
        },
        {
          nameLink: "CONTACT",
          active: "False",
          href: "#",
        },
        {
          nameLink: "MY ACCOUNT",
          active: "False",
          href: "#",
        },
      ],
    };
  },
};
</script>
<style lang="scss">
.bg-hero {
  background-image: url("../assets/hero-header-bakery.jpg");
  background-size: cover;
  background-position: center;
}
</style>