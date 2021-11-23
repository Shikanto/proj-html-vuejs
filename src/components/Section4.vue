<template>
  <div class="container">
    <div class="top-container-bakery-process d-flex">
      <img
        class="img-bakery-bg"
        :src="require('../assets/bakery-process-1.jpg')"
        alt=""
      />
      <div class="top-text d-flex">
        <h2>
          Tell us what you have in <br />
          mind
        </h2>
        <div class="number-process-bakery">01</div>
      </div>
      <div class="container-description d-flex align-end">
        <div class="subtitle text-start w-30">MANUAL INDREDIENTS SELECTION</div>
        <div class="description-text spacing-title text-start w-30">
          Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl
          varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis
          nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat,
          finibus in velit placerat, rutrum augue.
        </div>
      </div>
    </div>

    <div class="mid-container-bakery-process d-flex">
      <div class="container-start-baking d-flex">
        <img
          class="img-bakery-bg"
          :src="require('../assets/bakery-process-2.jpg')"
          alt=""
        />
        <div class="top-text d-flex">
          <h2>We Start Baking</h2>
          <div class="number-process-bakery">02</div>
        </div>
        <div class="container-description d-flex align-start">
          <div class="subtitle text-start">Sweet & Delicious</div>
          <div class="description-text spacing-title text-start w-40">
            Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl
            varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis
            sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec
            lorem erat, finibus in velit placerat.
          </div>
        </div>
      </div>
      <div class="container-cit">
        <div class="subtitle">DONT JUST TAKE OUR WORD FOR IT</div>
        <h2>
          "Finally found an alternative to the mass produced products. Something
          that incorporates real organic ingredients, nutrient dense wellness
          whiile promoting sustainability and activity."
        </h2>
        <div class="subtitle">RACHEL COOPER, FOUNDER</div>
      </div>
    </div>
    <div class="div"></div>
  </div>
</template>
<script>
export default {
  name: "Section4",
};
</script>
<style lang="scss">
</style>