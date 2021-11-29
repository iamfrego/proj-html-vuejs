<template>
  <div class="site_main">
    <ImageContainer url="h3-img-" svgUrl="svg-12" />
    <Banner />
    <Offers />
    <DoItYourself />
    <ImageContainer url="h1-team-" :people="people" />
    <Type />
    <Menu :pizze="pizze" />
    <Event />
    <Booking />
  </div>
</template>

<script>
import ImageContainer from "./ImageContainer";
import Banner from "./Banner";
import Offers from "./Offers";
import DoItYourself from "./DoItYourself";
import Type from "./Type.vue";
import Menu from "./Menu.vue";
import Event from "./Event.vue";
import Booking from "./Booking.vue";
export default {
  data() {
    return {
      pizze: [
        {
          img: "h3-product-img-1a-100x100.png",
          name: "VALDOSTANA",
          price: "€55",
        },
        {
          img: "h3-product-img-2a-150x150.png",
          name: "FIORI DI ZUCCA",
          price: "€50",
        },
        {
          img: "h3-product-img-3a-150x150.png",
          name: "CAMPAGNOLA",
          price: "€95",
        },
        {
          img: "h3-product-img-4a-150x150.png",
          name: "VALDOSTANA",
          price: "€55",
        },
        {
          img: "h3-product-img-5a-150x150.png",
          name: "FIORI DI ZUCCA",
          price: "€50",
        },
        {
          img: "h3-product-img-6a-100x100.png",
          name: "CAMPAGNOLA",
          price: "€95",
        },
      ],
      people: [
        { name: "Er Cannella" },
        { name: "Canta Gallo" },
        { name: "Chucky Beta" },
        { name: "Detective Conan" },
      ],
    };
  },
  components: {
    ImageContainer,
    Banner,
    Offers,
    DoItYourself,
    Type,
    Menu,
    Event,
    Booking,
  },
};
</script>

<style lang="scss" scoped></style>
