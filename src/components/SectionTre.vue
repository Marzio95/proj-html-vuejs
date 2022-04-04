<template>
  <div class="section">
    <div class="col_left">
      <img src="../assets/images/artist-quote-icon.png" alt="''" />
      <h1>
        I coach and mentor visual artists, like you, to Create Like You Mean It
      </h1>
      <div class="particular_text">Martin Garrix</div>
    </div>
    <div class="col_right">
      <div class="text">
        As a coach and mentor, my ultimate goal is to motivate visual artists
        toward inspired action. I help you get you vack on track to being the
        productive, creative, meaninful and authentic artist you truly want to
        be. I support artist in crafting and living a crative life as well as
        feeling good about themselves and their art.
      </div>
      <div class="text">
        Asn an artist ad educator for nearly 30 years, I understand what it
        takes to create.
      </div>
      <button>Get started today</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionTre",
};
</script>

<style scoped lang="scss">
.section {
  height: 560px;
  display: flex;
}
.col_left {
  width: 50%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 10rem;
  margin-left: 3rem;
}
.col_right {
  width: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-right: 2rem;
}
h1 {
  margin: 2.5rem 0;
  font-size: 2.5rem;
}
.text {
  color: gray;
  font-size: 1.4rem;
  margin: 0.5rem;
}
button {
  align-self: start;
  margin-top: 2rem;
  color: #efab43;
  background-color: #f4f0ef;
  padding: 1.2rem;
  width: 14rem;
  border: none;
  font-size: 1.1rem;
  font-weight: 800;
}
</style>
