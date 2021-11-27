<template>
  <div class="footer starred_background pt_footer_row">
    <div class="row row-cols-2">
      <div class="col">
        <div class="row row-cols-3">
          <div class="col ps-5">
            <h3>FIND OUR RESTAURANTS</h3>
            <div
              v-for="restaurant in restaurantList"
              :key="restaurant.Address"
              class="text-white py-3"
            >
              <p>{{ restaurant.Address }}</p>
              <p>{{ restaurant.City }}</p>
              <p>{{ restaurant.Phone }}</p>
            </div>
          </div>
          <div class="col">
            <div class="worktime">
              <h3>WORKING HOURS</h3>
              <div class="timetables">
                <div class="pt-3">
                  <p class="days">MONDAY</p>
                  <p class="freeday">{{ freeday }}</p>
                </div>
                <div class="pt-3">
                  <p class="days">TUESDAY UNTIL FRIDAY</p>
                  <p class="text-white">{{ weekday }}</p>
                </div>
                <div class="pt-3">
                  <p class="days">SATURDAY</p>
                  <p class="text-white">{{ longday }}</p>
                </div>
                <div class="pt-3">
                  <p class="days">SUNDAY</p>
                  <p class="text-white">{{ weekday }}</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col"></div>
        </div>
      </div>
      <div class="col"></div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    restaurantsArray: Array,
    freeday: String,
    weekday: String,
    longday: String,
  },
  data() {
    return {
      restaurantList: [],
    };
  },
  methods: {
    restaurantsDisplay() {
      this.restaurantsArray.forEach((restaurantList) => {
        this.restaurantList.push(restaurantList);
      });
      console.log(this.restaurantList);
    },
  },
  mounted() {
    this.restaurantsDisplay();
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";

.pt_footer_row {
  padding-top: 10rem;
}

h3,
.days {
  color: $color-third;
}
.freeday {
  color: $color-secondary;
}
</style>
