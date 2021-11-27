<template>
  <div class="event mt-5">
    <div class="row row-cols-2">
      <List
        :title="Title"
        :description="description"
        :array="Events"
        class="starred_background text-white"
      />
      <div
        class="col col_image d-flex justify-content-center align-items-center"
      >
        <div class="img">
          <img src="../assets/img/h3-img-5a.jpg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import List from "./List.vue";

export default {
  data() {
    return {
      Title: "DELISH PIZZA DEALS",
      description: "",
      Events: [
        {
          Id: "02",
          Date: "NOV",
          Title: "TRADITIONALE NEAPOLITAN PIES IN KYOTO PIZZA MERCATO",
          Description: "204 E. Pizzetta Tommaso",
        },
        {
          Id: "03",
          Date: "NOV",
          Title: "TERRAZZA PATIO DINING SPACE OPENING THIS WEEKEND",
          Description: "204 E. Pizzetta Tommaso",
        },
        {
          Id: "05",
          Date: "NOV",
          Title: "SIENNA PRIVATE DINING ROOM  WITH STEPHANE BRAUNN",
          Description: "204 E. Pizzetta Tommaso",
        },
      ],
    };
  },
  components: {
    List,
  },
};
</script>

<style lang="scss">
.col_image {
  img {
    width: 100%;
  }
}
</style>
