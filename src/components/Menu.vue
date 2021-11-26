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
    <div class="pizza_carousel d-flex justify-content-center mt-5">
      <div class="row row-cols-6">
        <div class="col" v-for="pizza in pizzaType" :key="pizza.img">
          <div class="card">
            <img :src="require('../assets/img/' + pizza.img)" alt="" />
            <h5 class="mt-4">{{ pizza.name }}</h5>
            <h5 class="price">{{ pizza.price }}</h5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    pizze: Array,
  },
  data() {
    return {
      pizzaType: [],
    };
  },
  methods: {
    pizzaList() {
      this.pizze.forEach((pizzaType) => {
        this.pizzaType.push(pizzaType);
      });
      console.log(this.pizzaType);
    },
  },
  mounted() {
    this.pizzaList();
  },
};
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
.pizza_carousel {
  .row {
    flex-wrap: nowrap;
    .card {
      border: 0;
      cursor: pointer;
      img {
        width: 300px;
      }
      h5 {
        color: $color-third;
        text-align: center;
      }
      .price {
        color: $color-secondary;
      }
    }
  }
}
</style>
