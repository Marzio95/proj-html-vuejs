<template>
  <main>
    <SectionUno />
    <SectionDue />
    <SectionTre />
    <SectionQuattro />
  </main>
</template>

<script>
import SectionUno from "./SectionUno.vue";
import SectionDue from "./SectionDue.vue";
import SectionTre from "./SectionTre.vue";
import SectionQuattro from "./SectionQuattro.vue";

export default {
  components: {
    SectionUno,
    SectionDue,
    SectionTre,
    SectionQuattro,
  },
  name: "MainProj",
};
</script>

<style scoped lang="scss"></style>
