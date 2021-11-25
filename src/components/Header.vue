<template>
  <div class="site_header">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-nav">
        <div class="navbar-collapse justify-content-center">
          <div class="container-nav-block d-flex justify-content-between">
            <div class="order">
              <button class="btn btn_order">ORDER ONLINE</button>
            </div>
            <ul class="navbar-nav">
              <li class="nav-item">
                <a class="nav-link text-white pe-3" href="#">
                  <img src="../assets/svg/svg-0.svg" alt="" /> HOME</a
                >
              </li>
              <li class="nav-item">
                <a class="nav-link text-white pe-3" href="#">PAGES</a>
              </li>
              <li class="nav-item">
                <a class="nav-link text-white pe-5" href="#">MENU</a>
              </li>
            </ul>
          </div>
          <img src="../assets/img/h5-logo-divided-header.png" alt="" />

          <div class="container-nav-block d-flex justify-content-between">
            <ul class="navbar-nav">
              <li class="nav-item">
                <a class="nav-link text-white ps-5 pe-3" href="#">EVENT</a>
              </li>
              <li class="nav-item">
                <a class="nav-link text-white pe-3" href="#">BLOG</a>
              </li>
              <li class="nav-item">
                <a class="nav-link text-white pe-3" href="#">LANDING</a>
              </li>
            </ul>
            <div class="cart_and_search">
              <ul class="navbar-nav">
                <li class="nav-item">
                  <a class="nav-link text-white pe-3" href="#">
                    <img
                      src="../assets/svg/svg-1.svg"
                      alt=""
                      class="pe-2"
                    />CART</a
                  >
                </li>
                <li class="nav-item">
                  <a class="nav-link text-white pe-3" href="#">
                    <i class="fas fa-search pe-2"></i>SEARCH</a
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
export default {};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";

.site_header {
  background-image: url("../assets/img/banner-starred.png");
  font-size: 13px;

  .container-nav-block {
    width: 500px;
  }

  .btn_order {
    font-size: 13px;
    color: white;
    background-color: $order-btn;
  }
  .navbar {
    padding: 0 0 !important;

    .container-nav {
      width: 100%;
      background-image: url("../assets/img/banner-starred.png");
      padding-top: 1rem;
      img {
        width: 150px;
      }
    }
    .nav-item {
      img {
        width: fit-content;
        height: 13px;
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
