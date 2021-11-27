<template>
  <body>
    <Header />
    <Main />
    <Footer
      :restaurantsArray="restaurants"
      :freeday="freeday"
      :weekday="weekday"
      :longday="longday"
    />
  </body>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  data() {
    return {
      restaurants: [
        {
          Address: "1614 E.Bell Rd #104",
          City: "Salerno, AZ 85022",
          Phone: "(602) 867-1010",
        },
        {
          Address: "204 E.Piazzetta Tommaso",
          City: "Sorrento, AZ 85022",
          Phone: "(602) 867-1010",
        },
        {
          Address: "Viale Puglia 54",
          City: "Torre Del Greco, AZ 85022",
          Phone: "(602) 867-1010",
        },
        {
          Address: "Corso Itali AA",
          City: "Naples, AZ 85022",
          Phone: "(602) 867-1010",
        },
      ],
      freeday: "Kitchen Closed",
      weekday: "9:00 - 22:00",
      longday: "11am to midnight",
    };
  },
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import "../node_modules/bootstrap/scss/bootstrap.scss";
@import url("https://fonts.googleapis.com/css2?family=Oswald:wght@100;400;600;700&display=swap");
@import "./assets/scss/commons.scss";

body {
  font-family: "Oswald", sans-serif;
  overflow-x: hidden;
}
</style>
