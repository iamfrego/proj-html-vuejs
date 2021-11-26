<template>
  <div class="menu mt-3">
    <div class="info">
      <p class="flavor">CHOOSE YOUR FLAVOR</p>
      <h1>THE BEST PIZZA MENU IN TOWN</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat ut
        perferendis, itaque consequuntur minima, modi fugit ad corporis, rem
        facilis quos! Tenetur, et eum exercitationem quas perferendis veniam
        provident explicabo.
      </p>
    </div>
    <div class="pizza_carousel"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";
.menu {
  .info {
    text-align: center;
    .flavor {
      font-size: 15px;
      color: $color-secondary;
    }
    h1 {
      font-weight: 900;
    }
    p {
      color: grey;
    }
  }
}
</style>
