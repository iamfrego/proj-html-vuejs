<template>
  <div class="offers mt-3">
    <div class="row row-cols-2">
      <div
        class="col col_image d-flex justify-content-center align-items-center"
      >
        <img src="../assets/img/h1-img-7n.png" alt="" />
      </div>
      <div class="col position-relative">
        <div class="container_combo position-absolute">
          <h3>SPECIALS*</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Est,
            molestias?
          </p>
          <div class="combo_list">
            <div class="row row-cols-2">
              <div class="col">
                <h3 class="combo_id">S10</h3>
              </div>
              <div class="col">
                <h3>COMBO PICCOLO</h3>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Mollitia, aspernatur!
                </p>
              </div>
            </div>
            <div class="row row-cols-2">
              <div class="col">
                <h3 class="combo_id">S20</h3>
              </div>
              <div class="col">
                <h3>COMBO MEDIO</h3>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Mollitia, aspernatur!
                </p>
              </div>
            </div>
            <div class="row row-cols-2">
              <div class="col">
                <h3 class="combo_id">S30</h3>
              </div>
              <div class="col">
                <h3>COMBO GRANDE</h3>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Mollitia, aspernatur!
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";

.col_image {
  background-image: url("../assets/img/h1-img-4.jpg");
  height: 800px;
  background-size: cover;
}

.container_combo {
  width: fit-content;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  h3 {
    font-weight: 700;
  }
  .combo_id {
    color: $color-secondary;
  }
}
.combo_list {
  .col {
    margin: auto;
    margin-top: 20px;
    width: fit-content;
  }
}
</style>
