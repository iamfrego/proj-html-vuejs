<template>
  <div class="site_main">
    <div class="img_container">
      <div class="row">
        <div class="col" v-for="n in 4" :key="n.i">
          <img :src="`../assets/img/h3-img-` + n + `.jpg`" alt="" />
        </div>
      </div>
    </div>
    <div class="banner"></div>
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
.img_container {
  height: 225px;
}
.banner {
  height: 400px;
  background-repeat: repeat-x;
  background-position-y: center;
  background-image: url("../assets/img/h3-testimonials-bckgrnd.jpg");
}
</style>
