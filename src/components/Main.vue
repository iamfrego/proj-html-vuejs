<template>
  <div class="site_main">
    <div class="img_container">
      <div class="row py-2 g-3">
        <div class="col-3" v-for="n in 4" :key="n.i">
          <img
            :src="require(`../assets/img/h3-img-` + n + `.jpg`)"
            alt=""
            class="img-fluid"
          />
        </div>
      </div>
    </div>
    <div
      class="
        banner
        d-flex
        justify-content-center
        align-items-center
        text-center
      "
    >
      <div class="text">
        <img src="../assets/img/virgolette.png" alt="" class="mx-auto mb-5" />
        <h3>
          <strong
            >"FORGET THE TRENDY PIZZA SHOP, THIS HIDDEN SPOT MAKES THE BEST NEW
            YORK-STYLE PIZZA SLICE IN NAPLES"</strong
          >
        </h3>
        <p>WASHINGTON POST 2018</p>
      </div>
    </div>
    <div class="offers"></div>
    <div class="banner2"></div>
    <div class="img_container"></div>
    <div class="type"></div>
    <div class="menu">
      <div class="info"></div>
      <div class="pizza_carousel"></div>
    </div>
    <div class="event"></div>
    <div class="booking"></div>
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
  .text {
    p {
      color: $color-secondary;
    }
    img {
      width: 100px;
    }
  }
}
</style>
