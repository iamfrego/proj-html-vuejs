<template>
  <div class="site_header starred_background">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-nav starred_background">
        <div class="navbar-collapse justify-content-center">
          <div class="container-nav-block d-flex justify-content-between">
            <div class="order">
              <button class="btn btn_order text-white">{{ button }}</button>
            </div>
            <ul class="navbar-nav">
              <li class="nav-item">
                <a class="nav-link text-white pe-3" href="#">
                  <img src="../assets/svg/svg-0.svg" alt="" /> {{ link1 }}</a
                >
              </li>
              <li class="nav-item">
                <a class="nav-link text-white pe-3" href="#">{{ link2 }}</a>
              </li>
              <li class="nav-item">
                <a class="nav-link text-white pe-5" href="#">{{ link3 }}</a>
              </li>
            </ul>
          </div>
          <img src="../assets/img/h5-logo-divided-header.png" alt="" />

          <div class="container-nav-block d-flex justify-content-between">
            <ul class="navbar-nav">
              <li class="nav-item">
                <a class="nav-link text-white ps-5 pe-3" href="#">{{
                  link4
                }}</a>
              </li>
              <li class="nav-item">
                <a class="nav-link text-white pe-3" href="#">{{ link5 }}</a>
              </li>
              <li class="nav-item">
                <a class="nav-link text-white pe-3" href="#">{{ link6 }}</a>
              </li>
            </ul>
            <div class="cart_and_search">
              <ul class="navbar-nav">
                <li class="nav-item">
                  <a class="nav-link text-white pe-3" href="#">
                    <img src="../assets/svg/svg-1.svg" alt="" class="pe-2" />{{
                      link7
                    }}</a
                  >
                </li>
                <li class="nav-item">
                  <a class="nav-link text-white pe-3" href="#">
                    <i class="fas fa-search pe-2"></i>{{ link8 }}</a
                  >
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <div class="jumbo text-center">
      <img src="../assets/img/h3-rev-img-6.png" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    button: String,
    link1: String,
    link2: String,
    link3: String,
    link4: String,
    link5: String,
    link6: String,
    link7: String,
    link8: String,
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";

.site_header {
  font-size: 20px;

  .container-nav-block {
    width: 500px;
  }

  .btn_order {
    font-size: 20px;
    background-color: $color-secondary;
  }
  .navbar {
    padding: 0 0 !important;

    .container-nav {
      width: 100%;
      padding-top: 1rem;
      img {
        width: 150px;
      }
    }
    .nav-item {
      img {
        width: fit-content;
        height: 17px;
        filter: invert(1);
      }
    }
  }
  .jumbo {
    background-image: url("../assets/img/h3-rev-img-5.png");
    background-repeat: no-repeat;
    background-position-x: center;
    height: 450px;
    img {
      height: 350px;
      margin: 30px;
    }
  }
}
</style>
