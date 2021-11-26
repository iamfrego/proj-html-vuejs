<template>
  <div class="offers mt-3">
    <div class="row row-cols-2">
      <BigImageCol :img="Image" />
      <List :title="Title" :description="description" :array="Combo" />
    </div>
  </div>
</template>

<script>
import BigImageCol from "./BigImageCol.vue";
import List from "./List.vue";
export default {
  data() {
    return {
      Image: "h1-img-7n.png",
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
    BigImageCol,
    List,
  },
};
</script>

<style lang="scss"></style>
