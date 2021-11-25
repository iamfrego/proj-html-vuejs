<template>
  <div class="site_main">
    <ImageContainer url="h3-img-" />
    <Banner />
    <Offers />
    <ImageContainer url="h1-team-" />

    <!-- <div class="banner2"></div>
    <div class="img_container"></div>
    <div class="type"></div>
    <div class="menu">
      <div class="info"></div>
      <div class="pizza_carousel"></div>
    </div>
    <div class="event"></div>
    <div class="booking"></div> -->
  </div>
</template>

<script>
import ImageContainer from "./ImageContainer";
import Banner from "./Banner";
import Offers from "./Offers";
export default {
  components: {
    ImageContainer,
    Banner,
    Offers,
  },
};
</script>

<style lang="scss" scoped></style>
