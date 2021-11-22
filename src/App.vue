<template>
  <div id="app">
    <Header>
    </Header>
    <main class="spacing-section">
      <Section1></Section1>
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import Section1 from "./components/Section1.vue"

export default {
  name: "App",
  components: {
    Header, Section1,
  },
};
</script>

<style lang="scss">
@import "style/app.scss";
</style>
