<template>
  <main>
    <SectionUno />
    <SectionDue />
  </main>
</template>

<script>
import SectionUno from "./SectionUno.vue";
import SectionDue from "./SectionDue.vue";

export default {
  components: {
    SectionUno,
    SectionDue,
  },
  name: "MainProj",
};
</script>

<style scoped lang="scss"></style>
