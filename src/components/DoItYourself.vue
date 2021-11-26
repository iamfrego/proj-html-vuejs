<template>
  <div class="doItYourself">
    <div class="container_text">
      <div class="text">
        <p class="text-white">
          GO AHED AND BUILD YOUR OWN PIZZA WE WON'T JUDGE!
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.doItYourself {
  background-image: url(/img/h3-background-img.3d6f30b4.jpg);
  height: 600px;
  background-position-y: 590px;
  background-position-x: center;
  position: relative;

  .container_text {
    height: 350px;
    width: 100%;
    background-image: url(/img/h3-background-img.3d6f30b4.jpg);
    background-position-x: center;
    background-position-y: -12.5rem;
    position: absolute;
    left: 0;
    top: 120px;
    background-size: cover;
    .text {
      width: 20%;
      margin-left: 15rem;
      p {
        font-size: 70px;
        position: relative;
        bottom: 2.5rem;
      }
    }
  }
}
</style>
