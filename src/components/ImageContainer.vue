<template>
  <div class="img_container mt-3">
    <div class="row py-2 g-3">
      <div class="col-3" v-for="n in 4" :key="n.i">
        <img
          :src="require('../assets/img/' + url + n + '.jpg')"
          alt=""
          class="img-fluid"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    url: String,
  },
};
</script>

<style></style>
