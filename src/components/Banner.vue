<template>
  <div
    class="
      banner
      mt-3
      d-flex
      justify-content-center
      align-items-center
      text-center
      position-relative
    "
  >
    <div class="text">
      <img src="../assets/img/virgolette.png" alt="" class="mx-auto mb-5" />
      <h3 class="mx-auto">
        <strong
          >"FORGET THE TRENDY PIZZA SHOP, THIS HIDDEN SPOT MAKES THE BEST NEW
          YORK-STYLE PIZZA SLICE IN NAPLES"</strong
        >
      </h3>
      <p>WASHINGTON POST 2018</p>
    </div>
    <img src="../assets/svg/svg-4.svg" alt="" class="position-absolute" />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";

.banner {
  height: 400px;
  background-position-y: center;
  background-image: url("../assets/img/h3-testimonials-bckgrnd.jpg");
  img {
    right: 30px;
    bottom: 30px;
  }
  .text {
    h3 {
      width: 70%;
    }
    p {
      color: $color-secondary;
    }
    img {
      width: 100px;
    }
  }
}
</style>
