<template>
  <button class="button_orange">{{ text }}</button>
</template>

<script>
export default {
  name: "ButtonOrange",
  props: {
    text: String,
  },
};
</script>

<style scoped lang="scss">
.button_orange {
  padding: 0.5rem;
  color: white;
  border: none;
  border-radius: 7px;
  font-weight: 600;
  background-color: #ec601c;
  width: 10rem;
}
.button_orange:hover {
  background-color: #b1e4f4;
}
</style>
