<template>
  <div class="type mt-4">
    <div class="row py-2 g-3 justify-content-center">
      <div class="col-2" v-for="n in 5" :key="n.i">
        <img
          :src="require('../assets/img/h1-clients-img-' + n + '.png')"
          alt=""
          class="img-fluid"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.type {
  background-color: #f7f7f2;
}
</style>
