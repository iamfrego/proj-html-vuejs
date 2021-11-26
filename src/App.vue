<template>
  <body>
    <Header />
    <Main />
  </body>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";

export default {
  components: {
    Header,
    Main,
  },
};
</script>

<style lang="scss">
@import "../node_modules/bootstrap/scss/bootstrap.scss";
@import url("https://fonts.googleapis.com/css2?family=Oswald:wght@100;400;600;700&display=swap");

body {
  font-family: "Oswald", sans-serif;
  overflow-x: hidden;
}
</style>
