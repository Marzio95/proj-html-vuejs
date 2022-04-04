<template>
  <section>
    <div class="center">
      <div class="particular_text">Artist coaching</div>
      <h2>Latest Online Courses</h2>
    </div>
    <div class="row">
      <div class="card" v-for="card in arrayCards" :key="card.title">
        <img :src="require('../assets/images/' + card.img)" alt="" />
        <div class="left">
          <div class="price">{{ card.price }}</div>
          <h3>{{ card.title }}</h3>
          <small>{{ card.lessons }} {{ card.students }}</small>
        </div>
      </div>
    </div>
    <div class="button_center">
      <button>View all courses</button>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionSei",
  data() {
    return {
      arrayCards: [
        {
          img: "artist-course-08-480x480.jpg",
          price: "$18.00",
          title: "The Acrylic Painting Academy",
          lessons: "4 Lessons",
          students: "50 Students",
        },
        {
          img: "artist-course-07-480x480.jpg",
          price: "$21.00",
          title: "Drawing and Shading: Complete Copurse",
          lessons: "14 Lessons",
          students: "50 Students",
        },
        {
          img: "artist-course-06-480x480.jpg",
          price: "$19.00",
          title: "The Color Theory fo Digital Artist",
          lessons: "7 Lessons",
          students: "50 Students",
        },
        {
          img: "artist-course-05-480x480.jpg",
          price: "$35.00",
          title: "Ultimate Guide to Digital Sketching for Beginner",
          lessons: "14 Lessons",
          students: "50 Students",
        },
        {
          img: "artist-course-04-480x480.jpg",
          price: "$19.00",
          title: "Portait Drawing The Smart Way",
          lessons: "2 Lessons",
          students: "50 Students",
        },
        {
          img: "artist-course-03-480x480.jpg",
          price: "$19.00",
          title: "Mastering Watercolor Painting from Beginner",
          lessons: "9 Lessons",
          students: "50 Students",
        },
        {
          img: "artist-course-02-480x480.jpg",
          price: "$25.00",
          title: "The Art & Science of Drawing",
          lessons: "4 Lessons",
          students: "50 Students",
        },
        {
          img: "artist-course-01-480x480.jpg",
          price: "$22.00",
          title: "The Colored Pencil Drawing Courdse",
          lessons: "6 Lessons",
          students: "50 Students",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.center {
  text-align: center;
  margin-top: 3rem;
  margin-bottom: 1.5rem;
}
h2 {
  margin-top: 1rem;
}
.row {
  display: flex;
  flex-wrap: wrap;
  margin: auto;
  width: 90%;
}
.card {
  width: calc(100% / 4);
  padding: 0.2rem;
  margin-bottom: 2rem;
}
.card:hover .left {
  border: 1px solid orangered;
  transform: translateY(-5rem);
  background-color: white;
  opacity: 1;
}
.left {
  padding: 1rem 0;
  padding-left: 1rem;
  opacity: 0.8;
  width: 73%;
  border: 1px solid transparent;
  height: 150px;
  background-color: white;
}
img {
  width: 300px;
  height: 300px;
}
.price {
  color: orangered;
  font-weight: 800;
}
h3 {
  margin: 1rem 0;
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
button:hover {
  background-color: orangered;
  color: white;
}
.button_center {
  text-align: center;
}
</style>
