<template>
  <div class="col col_image d-flex justify-content-center align-items-center">
    <img :src="require('../assets/img/' + img)" alt="" />
  </div>
</template>

<script>
export default {
  props: {
    img: String,
  },
};
</script>

<style>
.col_image {
  background-image: url("../assets/img/h1-img-4.jpg");
  height: 800px;
  background-size: cover;
}
</style>
