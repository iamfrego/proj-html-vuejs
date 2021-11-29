<template>
  <div class="img_container mt-3">
    <div class="row py-2 g-3">
      <div class="col-3" v-for="n in 4" :key="n.i">
        <div class="image">
          <img
            :src="require('../assets/img/' + url + n + '.jpg')"
            alt=""
            class="img-fluid card_image"
          />
          <img
            :src="require('../assets/svg/' + svgUrl + '.svg')"
            alt=""
            class="img-fluid card_image_hover"
            v-if="svgUrl"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    url: String,
    svgUrl: String,
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";

.col-3 {
  position: relative;

  .image {
    background-image: url("../assets/img/hover-background.jpg");
    position: relative;
    &:hover {
      .card_image {
        visibility: hidden;
      }
      .card_image_hover {
        visibility: visible;
      }
    }
    .card_image_hover {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      visibility: hidden;
    }
  }
}
</style>
