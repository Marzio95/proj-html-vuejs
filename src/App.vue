<template>
  <div id="app">
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
}
</style>
