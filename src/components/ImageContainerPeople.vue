<template>
  <div class="img_container mt-3">
    <div class="row py-2 g-3">
      <div class="col-3" v-for="(pp, n) in people" :key="pp.n">
        <div class="image">
          <img
            :src="require('../assets/img/' + url + (n + 1) + '.jpg')"
            alt=""
            class="img-fluid card_image"
          />
          <div
            class="
              details
              text-center text-white
              d-flex
              flex-column
              justify-content-center
            "
          >
            <h4>{{ pp.name }}</h4>
            <p>Kitchen Porter</p>
            <div class="icon">
              <i class="fab fa-instagram pe-2"></i>
              <i class="fab fa-twitter pe-2"></i>
              <i class="fab fa-facebook-f pe-2"></i>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    url: String,
    people: Array,
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

    .details {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      height: 250px;
      width: 250px;
      background-color: $color-secondary;
      visibility: hidden;
    }
    &:hover {
      .card_image {
        visibility: hidden;
      }
      .details {
        visibility: visible;
      }
    }
  }
}
</style>
