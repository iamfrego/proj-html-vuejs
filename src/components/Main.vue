<template>
  <div class="site_main">
    <ImageContainer url="h3-img-" />
    <Banner />
    <Offers />
    <DoItYourself />
    <ImageContainer url="h1-team-" />

    <!--   <div class="img_container"></div>
    <div class="type"></div>
    <div class="menu">
      <div class="info"></div>
      <div class="pizza_carousel"></div>
    </div>
    <div class="event"></div>
    <div class="booking"></div>  -->
  </div>
</template>

<script>
import ImageContainer from "./ImageContainer";
import Banner from "./Banner";
import Offers from "./Offers";
import DoItYourself from "./DoItYourself";
export default {
  components: {
    ImageContainer,
    Banner,
    Offers,
    DoItYourself,
  },
};
</script>

<style lang="scss" scoped></style>
