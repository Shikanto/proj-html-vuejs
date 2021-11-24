<template>
  <li>
    <a :href="`${infoLink.href}`">{{ infoLink.nameLink }}{{ infoLink.linkName }}</a>
  </li>
</template>
<script>
export default {
  name: "NavLinks",
  props: {
    infoLink: Object,
  },
};
</script>
<style lang="scss">

</style>