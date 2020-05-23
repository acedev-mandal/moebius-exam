<template>
  <div id="app">
    <HomePage />
  </div>
</template>

<script>
import HomePage from "./views/HomePage.vue";

export default {
  name: "App",
  components: {
    HomePage,
  },
};
</script>

<style lang="scss">
@import url(./assets/css/css-reset.css);
@import url(./assets/css/normalize.css);
@import url(./assets/css/font-family.css);

#app {
  font-family: "Rubik", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #f4f4fa;

  a {
    text-decoration: none;
  }
  .fl-left {
    float: left;
  }
  .fl-right {
    float: right;
  }
  .fine-line {
    border-top: solid 1px rgba(151, 151, 151, 0.18);
    padding-top: 79px;
  }
}
</style>
