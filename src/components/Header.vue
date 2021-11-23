<template>
  <header class="bg-hero">
    <div class="navBar d-flex">
      <div class="logo">
        <img :src="require('../assets/avada-bakery-logo.png')" alt="" />
      </div>
      <div class="container-navLinks">
          <ul class="d-flex">
            <NavLinks v-for="(link, i) in linksNavBar" 
            :key="i" :infoLink="link">
            </NavLinks>
            <li><a href="#"><i class="fa fa-shopping-cart" aria-hidden="true"></i></a></li>
        </ul>
      </div>
    </div>
    <div class="demosOnSale d-flex">
        <div class="container-demos d-flex">
            <div class="container-icon-demos d-flex">
                <div class="demos-sale"><i class="fa fa-database" aria-hidden="true"></i></div>
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
    <div class="container">
        <div class="hero">
            <div class="subtitle">
                FRESH & TASTY BAKERY EVERY DAY
            </div>
            <div class="spacing-title"><h1>The Perfect Fresh Bread</h1></div>
            <div class="text-hero">
                Cras consequat lectus vestibulum tortor pulvinar, quis 
                euismod nisl varius. Aliquam erat volutpat. Nullam quis 
                sagittis nibh ac nulla id orci tempor.
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
          nameLink: "Home",
          active: "True",
          href: "#",
        },
        {
          nameLink: "Shop",
          active: "False",
          href: "#",
        },
        {
          nameLink: "About",
          active: "False",
          href: "#",
        },
        {
          nameLink: "Gallery",
          active: "False",
          href: "#",
        },
        {
          nameLink: "Locations",
          active: "False",
          href: "#",
        },
        {
          nameLink: "Journal",
          active: "False",
          href: "#",
        },
        {
          nameLink: "Contact",
          active: "False",
          href: "#",
        },
        {
          nameLink: "My account",
          active: "False",
          href: "#",
        },
      ],
    };
  },
};
</script>
<style lang="scss">

.bg-hero{
    background-image: url("../assets/hero-header-bakery.jpg");
}
</style>