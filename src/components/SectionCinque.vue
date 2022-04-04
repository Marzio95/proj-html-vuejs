<template>
  <section>
    <div class="center">
      <div class="particular_text">Testimonials</div>
      <h2>Why do people love me?</h2>
    </div>
    <div class="row">
      <div class="card" v-for="card in arrayCard" :key="card.title">
        <h3>{{ card.title }}</h3>
        <p>{{ card.text }}</p>
        <div class="inline">
          <img :src="require('../assets/images/' + card.img)" alt="" />
          <div class="f_col">
            <h5>{{ card.name }}</h5>
            <h6>{{ card.role }}</h6>
          </div>
        </div>
      </div>
    </div>
    <div class="row_points">
      <div
        class="point"
        v-for="(point, index) in arrayPoints"
        :key="index"
      ></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionCinque",
  data() {
    return {
      arrayCard: [
        {
          title: "It's a choice of quality for people with special needs",
          text: "I'm a very strict person so i require everything to be organized and neat. Then, i'll be able to make things right and shine. MaxCoach guys just got me.",
          img: "artist-testimonial-avatar-02.jpg",
          name: "Florence Themes",
          role: "/ Multimedia Admin",
        },
        {
          title: "High level of efficiency and scientific teaching methods",
          text: "I am a free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal for people like me.",
          img: "artist-testimonial-avatar-04.jpg",
          name: "Mina Hollace",
          role: "/ Freelancer",
        },
        {
          title:
            "Professional team of specialists and passionate mentors at reach",
          text: "I need to get a certificatee for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
          img: "artist-testimonial-avatar-01.jpg",
          name: "Madley Pondor",
          role: "/ IT Specialist",
        },
      ],
      arrayPoints: [1, 2, 3],
    };
  },
};
</script>

<style scoped lang="scss">
section {
  background-color: #faf8f5;
}
.center {
  text-align: center;
  margin-top: 4rem;
  padding-top: 3rem;
  margin-bottom: 1rem;
}
.row {
  display: flex;
  justify-content: center;
}
.card {
  width: 30%;
  height: 330px;
  margin: 2rem;
  background-color: white;
  padding: 3rem;
}
p {
  margin: 2rem 0;
  color: gray;
}
img {
  height: 5rem;
  border-radius: 50%;
  margin-right: 1rem;
}
.inline {
  display: flex;
  align-items: center;
}
h6 {
  margin-top: 1rem;
}
.card:nth-child(1) {
  opacity: 0.4;
}
.card:nth-child(3) {
  opacity: 0.4;
}
.row_points {
  display: flex;
  justify-content: center;
  margin-top: 1rem;
  padding-bottom: 3rem;
}
.point {
  width: 1rem;
  height: 1rem;
  border-radius: 50%;
  background-color: gray;
  margin: 0 0.5rem;
}
.point:nth-child(1) {
  opacity: 0.4;
}
.point:nth-child(3) {
  opacity: 0.4;
}
</style>
