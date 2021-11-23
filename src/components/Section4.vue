<template>
  <div class="container">
    <div class="top-container-bakery-process d-flex bg-top-backery-process">
      <div class="top-text d-flex indexPlus">
        <h2>
          Tell us what you have in <br />
          mind
        </h2>
        <div class="number-process-bakery">01</div>
      </div>
      <div class="container-description d-flex align-end indexPlus">
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
      <div class="container-start-baking d-flex bg-mid-backery-process">
        <div class="top-text d-flex indexPlus">
          <h2>We Start Baking</h2>
          <div class="number-process-bakery">02</div>
        </div>
        <div class="container-description d-flex align-start indexPlus">
          <div class="subtitle text-start">Sweet & Delicious</div>
          <div class="description-text spacing-title text-start w-40">
            Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl
            varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis
            sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec
            lorem erat, finibus in velit placerat.
          </div>
        </div>
      </div>
      <div class="container-cit d-flex">
        <div class="subtitle">DONT JUST TAKE OUR WORD FOR IT</div>
        <h2 class="spacing-title">
          "Finally found an alternative to the mass produced products. Something
          that incorporates real organic ingredients, nutrient dense wellness
          whiile promoting sustainability and activity."
        </h2>
        <div class="subtitle">RACHEL COOPER, FOUNDER</div>
      </div>
    </div>

    <div class="bot-container-bakery-process">
      <div class="d-flex bg-bot-backery-process">
        <div class="top-text d-flex indexPlus">
          <h2>
            Tell us what you have in <br />
            mind
          </h2>
          <div class="number-process-bakery">03</div>
        </div>
        <div class="container-description d-flex indexPlus">
          <div class="subtitle text-start w-30">
            MANUAL INDREDIENTS SELECTION
          </div>
          <div class="description-text spacing-title text-start w-30">
            Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl
            varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis
            sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec
            lorem erat, finibus in velit placerat, rutrum augue.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Section4",
};
</script>
<style lang="scss">
.container {
  position: relative;
}

.bg-top-backery-process {
  background-image: url("../assets/bakery-process-1.jpg");
  background-size: cover;
}

.bg-mid-backery-process {
  background-image: url("../assets/bakery-process-2.jpg");
  background-size: cover;
}

.bg-bot-backery-process {
  background-image: url("../assets/bakery-process-3.jpg");
  background-size: cover;
  height: 100%;
  flex-direction: column;
  padding: 60px 70px;
  justify-content: space-between;
}

.bg-top-backery-process:before,
.bg-mid-backery-process:before,
.bg-bot-backery-process:before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  background: rgba(0, 0, 0, 0.3);
}
</style>