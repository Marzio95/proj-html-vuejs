<template>
  <main>
    <SectionUno />
    <SectionDue />
    <SectionTre />
    <SectionQuattro />
    <SectionCinque />
    <SectionSei />
    <SectionSette />
    <SectionOtto />
  </main>
</template>

<script>
import SectionUno from "./SectionUno.vue";
import SectionDue from "./SectionDue.vue";
import SectionTre from "./SectionTre.vue";
import SectionQuattro from "./SectionQuattro.vue";
import SectionCinque from "./SectionCinque.vue";
import SectionSei from "./SectionSei.vue";
import SectionSette from "./SectionSette.vue";
import SectionOtto from "./SectionOtto.vue";

export default {
  components: {
    SectionUno,
    SectionDue,
    SectionTre,
    SectionQuattro,
    SectionCinque,
    SectionSei,
    SectionSette,
    SectionOtto,
  },
  name: "MainProj",
};
</script>

<style scoped lang="scss"></style>
