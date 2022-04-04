<template>
  <section>
    <img src="../assets/images/artist-shape-color-paint-top-left.png" alt="" />
    <h2>
      Newsletter to get <br />
      in touch
    </h2>
    <input type="email" placeholder="Your e-mail" />
    <img
      src="../assets/images/artist-shape-color-paint-bottom-right.png"
      alt=""
    />
  </section>
</template>

<script>
export default {
  name: "SectionNove",
};
</script>

<style scoped lang="scss">
section {
  margin-top: 4rem;
  height: 200px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #22437d;
  color: white;
}
img {
  height: 200px;
}
h2 {
  text-align: end;
}
input {
  background-color: transparent;
  border: none;
  border-bottom: 1px solid white;
  width: 25rem;
  height: 2rem;
  color: white;
  font-size: 1.3rem;
}
textarea:focus,
input:focus {
  outline: none;
}
input::placeholder {
  color: white;
  font-size: 1.3rem;
}
</style>
