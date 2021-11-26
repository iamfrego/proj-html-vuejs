<template>
  <div class="offers mt-3">
    <div class="row row-cols-2">
      <div
        class="col col_image d-flex justify-content-center align-items-center"
      >
        <div class="img">
          <img src="../assets/img/h1-img-7n.png" alt="" />
        </div>
      </div>
      <List :title="Title" :description="description" :array="Combo" />
    </div>
  </div>
</template>

<script>
import List from "./List.vue";
export default {
  data() {
    return {
      Title: "SPECIALS*",
      description:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, molestias?",
      Combo: [
        {
          Id: "S10",
          Date: "",
          Title: "COMBO PICCOLO",
          Description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia, aspernatur!",
        },
        {
          Id: "S20",
          Date: "",
          Title: "COMBO MEDIO",
          Description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia, aspernatur!",
        },
        {
          Id: "S30",
          Date: "",
          Title: "COMBO GRANDE",
          Description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia, aspernatur!",
        },
      ],
    };
  },
  components: {
    List,
  },
};
</script>

<style scoped lang="scss">
.col_image {
  background-image: url("../assets/img/h1-img-4.jpg");
  height: 600px;
  background-size: cover;
  img {
    height: 400px;
  }
}
</style>
