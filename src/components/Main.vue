<template>
  <div class="site_main">
    <ImageContainer url="h3-img-" />
    <Banner />
    <Offers />
    <DoItYourself />
    <ImageContainer url="h1-team-" />
    <Type />
    <Menu />
    <!-- <div class="event"></div> -->
    <!-- <div class="booking"></div> -->
  </div>
</template>

<script>
import ImageContainer from "./ImageContainer";
import Banner from "./Banner";
import Offers from "./Offers";
import DoItYourself from "./DoItYourself";
import Type from "./Type.vue";
import Menu from "./Menu.vue";
export default {
  components: {
    ImageContainer,
    Banner,
    Offers,
    DoItYourself,
    Type,
    Menu,
  },
};
</script>

<style lang="scss" scoped></style>
