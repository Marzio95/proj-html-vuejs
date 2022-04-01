<template>
  <main>
    <SectionUno />
    <SectionDue />
    <SectionTre />
  </main>
</template>

<script>
import SectionUno from "./SectionUno.vue";
import SectionDue from "./SectionDue.vue";
import SectionTre from "./SectionTre.vue";

export default {
  components: {
    SectionUno,
    SectionDue,
    SectionTre,
  },
  name: "MainProj",
};
</script>

<style scoped lang="scss"></style>
