<template>
  <div class="booking">
    <div
      class="
        booking_input
        d-flex
        align-items-center
        justify-content-between
        py-5
      "
    >
      <select name="" id="" class="m-4 p-3">
        <option value="n" v-for="n in 20" :key="n">{{ n }} Persone</option>
      </select>
      <span class="text-white"><strong>FOR</strong></span>
      <input type="date" name="" id="" class="p-3" />
      <span class="text-white"><strong>AT</strong></span>
      <input type="time" name="" id="" class="p-3" />
      <button class="btn text-white p-3">BOOOK A TABLE</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";

.booking {
  background-image: url("../assets/img/h3-background-img-3.jpg");
  .booking_input {
    width: 45%;
    margin: auto;
    button {
      background-color: $color-secondary;
    }
  }
}
</style>
