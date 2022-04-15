<template>
  <div class="container">
    <div class="left_section">
      <img
        class="quadro"
        src="../assets/images/artist-course-01-480x480.jpg"
        alt="quadro"
      />
      <img
        class="monkey"
        src="../assets/images/artist-hero-image-01.jpg"
        alt="monkey"
      />
      <img
        class="afro"
        src="../assets/images/artist-hero-image-03.png"
        alt="afro"
      />
      <!-- <img
        class="blue"
        src="../assets/images/artist-hero-image-01.jpg"
        alt="blue"
      /> -->
      <img
        class="points"
        src="../assets/images/artist-shape-03.png"
        alt="points"
      />
    </div>
    <div class="center_section">
      <div class="particular_text">Hello Im Martin</div>
      <h2 class="main_text">Artist Coaching And Mentoring Might Be for You.</h2>
      <!-- <button class="ticket">Get started today</button> -->
      <button-orange class="button_plus" :text="text"></button-orange>
    </div>
    <div class="righ_section">
      <img
        class="martin"
        src="../assets/images/artist-hero-image-04.jpg"
        alt="martin"
      />
      <img
        class="macchia"
        src="../assets/images/artist-shape-01.png"
        alt="macchia"
      />
      <img
        class="pennello"
        src="../assets/images/artist-shape-05.png"
        alt="pennello"
      />
    </div>
  </div>
</template>

<script>
import ButtonOrange from "./ButtonOrange.vue";
export default {
  components: { ButtonOrange },
  name: "SectionUno",
  data() {
    return {
      text: "Get started today",
    };
  },
};
</script>

<style scoped lang="scss">
.container {
  min-height: 700px;
  display: flex;
  align-items: center;
  background-color: #faf8f5;
}
.left_section {
  width: 35%;
  position: relative;
  height: 100%;
}
.center_section {
  width: 30%;
  text-align: center;
  z-index: 9000;
}
.right_section {
  width: 35%;
  position: relative;
  height: 100%;
}
// .ticket {
//   padding: 0.7rem;
//   color: white;
//   border: none;
//   border-radius: 7px;
//   font-weight: 600;
//   background-color: #ec601c;
//   width: 12rem;
// }
// .ticket:hover {
//   background-color: #b1e4f4;
// }
.button_plus {
  width: 12rem !important;
  padding: 0.7rem !important;
}
.main_text {
  margin-top: 1rem;
  margin-bottom: 3rem;
}
.quadro {
  width: 200px;
  height: 300px;
  position: absolute;
  left: 17rem;
  top: 3rem;
  overflow: hidden;
  z-index: 1;
}
.monkey {
  position: absolute;
  left: 6rem;
  bottom: 3rem;
  overflow: hidden;
  z-index: 2;
}
.afro {
  position: absolute;
  right: -3rem;
  bottom: 0rem;
  z-index: 0;
}
.martin {
  position: absolute;
  right: 7rem;
  bottom: 5rem;
  overflow: hidden;
  z-index: 3;
}
.pennello {
  position: absolute;
  right: 0rem;
  bottom: 3rem;
  z-index: 1;
  overflow: hidden;
}
.macchia {
  position: absolute;
  right: 3rem;
  bottom: 3rem;
  overflow: hidden;
  object-fit: contain;
  height: 75%;
}
</style>
