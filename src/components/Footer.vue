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
          <div class="col d-flex flex-column">
            <div class="worktime">
              <h3>WORKING HOURS</h3>
              <div class="timetables">
                <div class="pt-3">
                  <p class="section_title">MONDAY</p>
                  <p class="freeday">{{ freeday }}</p>
                </div>
                <div class="pt-3">
                  <p class="section_title">TUESDAY UNTIL FRIDAY</p>
                  <p class="text-white">{{ weekday }}</p>
                </div>
                <div class="pt-3">
                  <p class="section_title">SATURDAY</p>
                  <p class="text-white">{{ longday }}</p>
                </div>
                <div class="pt-3">
                  <p class="section_title">SUNDAY</p>
                  <p class="text-white">{{ weekday }}</p>
                </div>
              </div>
            </div>
            <div class="social d-flex">
              <p class="section_title pe-3">FOLLOW US:</p>
              <div class="social_icon text-white">
                <i class="fab fa-twitter pe-2"></i>
                <i class="fab fa-facebook-f pe-2"></i>
                <i class="fab fa-instagram pe-2"></i>
                <i class="fab fa-linkedin-in pe-2"></i>
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
.section_title {
  color: $color-third;
}
.freeday {
  color: $color-secondary;
}
</style>
