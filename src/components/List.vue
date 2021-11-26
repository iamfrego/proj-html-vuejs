<template>
  <div class="col position-relative">
    <div class="container_list position-absolute">
      <h3>{{ title }}</h3>
      <p>{{ description }}</p>
      <div class="list">
        <div class="row row-cols-2" v-for="item in arrayObject" :key="item.i">
          <div class="col">
            <h3 class="list_id">{{ item.Id }}</h3>
            <h4 class="text-center">{{ item.Date }}</h4>
          </div>
          <div class="col">
            <h3>{{ item.Title }}</h3>
            <p>
              {{ item.Description }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    description: String,
    array: Array,
  },

  data() {
    return {
      arrayObject: [],
    };
  },
  methods: {
    arrayList() {
      this.array.forEach((arrayObject) => {
        this.arrayObject.push(arrayObject);
      });
    },
  },
  mounted() {
    this.arrayList();
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";

.container_list {
  width: fit-content;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  h3 {
    font-weight: 700;
  }
  p {
    color: gray;
  }
  .list_id {
    color: $color-secondary;
  }
}
.list {
  .col {
    margin: auto;
    margin-top: 20px;
    width: fit-content;
  }
}
</style>
