<template>
<footer>
    <div class="container">
        <div class="top-footer d-flex">
            <div class="left-top-footer">
                <div class="spacing-title">
                    <img :src="require('../assets/avada-bakery-logo.png')" alt="" />
                </div>
                <div class="navBar">
                    <ul class="d-flex">
                        <NavLinks v-for="(link, i) in linksNavBar" 
                        :key="i" :infoLink="link">
                        </NavLinks>
                        <li>
                            <a href="#">
                                <i class="fa fa-shopping-cart" aria-hidden="true">
                                <span class="number-item">0</span></i>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="right-top-footer text-end">
                <h3 class="spacing-title">Subscribe to our Newsletter</h3>
                <div class="d-flex gap">
                    <input class="input-email" type="text" placeholder="Enter email address*">
                    <button class="btn btn-purple">Subscribe</button>
                </div>
            </div>
        </div>
        <div class="bot-footer d-flex">
            <div class="subtitle">&#169; Copyright 2012 - 2020 | Avada Theme by
                ThemeFusion | All Rights Reserved | Powere by WordPress
            </div>
            <div class="list-social d-flex">
                <a href="#"><i class="fa fa-instagram" aria-hidden="true"></i></a>
                <a href="#"><i class="fa fa-twitter" aria-hidden="true"></i></a>
                <a href="#"><i class="fa fa-facebook" aria-hidden="true"></i></a>
                <a href="#"><i class="fa fa-pinterest-p" aria-hidden="true"></i></a>
            </div>
        </div>
    </div>
</footer>
</template>
<script>
import NavLinks from "./NavLinks.vue";

export default {
    name:"Footer",
    components:{
        NavLinks,
    },
    data() {
    return {
      linksNavBar: [
        {
          linkName: "Shop",
          href: "#",
        },
        {
          linkName: "About",
          href: "#",
        },
        {
          linkName: "Gallery",
          href: "#",
        },
        {
          linkName: "Locations",
          href: "#",
        },
        {
          linkName: "Journal",
          href: "#",
        },
        {
          linkName: "Contact",
          href: "#",
        },
        {
          linkName: "Orders",
          href: "#",
        },
      ],
    };
  },
}
</script>
<style lang="scss">
    
</style>