<template>
  <section class="section">
    <div class="top_section">
      <div class="particular_text">Artist coaching</div>
      <h2 class="main_text">
        I understand what it takes to create. <br />
        I can help you with
      </h2>
    </div>
    <div class="bottom_section">
      <div class="card" v-for="card in arrayConsigli" :key="card.title">
        <img
          :src="require('../assets/images/' + card.image)"
          :alt="card.image"
        />
        <h4>{{ card.title }}</h4>
        <div>{{ card.text }}</div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionDue",
  data() {
    return {
      arrayConsigli: [
        {
          image: "artist-box-image-01.png",
          title: "Online Corses",
          text: "Online art coaching now offers you a very powerful  way to redesign your mind.",
        },
        {
          image: "artist-box-image-02.png",
          title: "One to One",
          text: "Getting the necessary clarity about the current state to help you improve your ability.",
        },
        {
          image: "artist-box-image-03.png",
          title: "Anywhere",
          text: "Access to valuable and portable program which allow you to setup and live anywhere you want.",
        },
        {
          image: "artist-box-image-04.png",
          title: "On time",
          text: "Punctually is our top priority because it's on essential criteria to assess a program  quality.",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.section {
  background-image: url(../assets/images/maxcoach-shape-03.png);
  background-position-y: bottom;
  min-height: 440px;
}
.top_section {
  text-align: center;
  margin: 3rem 0;
}
.main_text {
  margin-top: 1rem;
  margin-bottom: 3rem;
}
.bottom_section {
  width: 80%;
  margin: auto;
  display: flex;
}
.card {
  padding: 1rem;
}
.bottom_section .card:last-child {
  margin-bottom: -5rem;
}
h4 {
  margin: 1rem 0;
}
</style>
