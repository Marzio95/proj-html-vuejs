<template>
  <div id="app">
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Monsieur+La+Doulaise&display=swap"
      rel="stylesheet"
    />
    <HeaderProj />
    <MainProj />
    <FooterProj />
  </div>
</template>

<script>
import HeaderProj from "./components/HeaderProj.vue";
import MainProj from "./components/MainProj.vue";
import FooterProj from "./components/FooterProj.vue";

export default {
  name: "App",
  components: {
    HeaderProj,
    MainProj,
    FooterProj,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
  scroll-behavior: smooth;
}
.particular_text {
  color: #029fcc;
  font-family: "Monsieur La Doulaise", cursive;
  font-size: 4rem;
}
button {
  cursor: pointer;
}
a {
  text-decoration: none;
  color: black;
}
#app {
  min-width: 1370px;
}
</style>
