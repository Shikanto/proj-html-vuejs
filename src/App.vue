<template>
  <div id="app">
    <Header>
    </Header>
    <main >
      <Section1 class="spacing-section"></Section1>
      <Section2 class="spacing-section"></Section2>
      <Section3 class="spacing-section"></Section3>
      
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import Section1 from "./components/Section1.vue"
import Section2 from "./components/Section2.vue"
import Section3 from "./components/Section3.vue"

export default {
  name: "App",
  components: {
    Header, Section1, Section2, Section3,
  },
};
</script>

<style lang="scss">
@import "style/app.scss";
</style>
