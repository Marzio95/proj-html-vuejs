<template>
  <section>
    <div class="center">
      <div class="particular_text">Upcoming Events</div>
      <h2>Let's Work Together</h2>
    </div>
    <div class="row_top">
      <div class="card" v-for="card in arrayCardsTop" :key="card.title">
        <div class="col_left">
          <img :src="require('../assets/images/' + card.img)" alt="" />
        </div>
        <div class="col_right">
          <h6>{{ card.calendar }}</h6>
          <h3>{{ card.title }}</h3>
          <small>{{ card.position }}</small>
        </div>
      </div>
    </div>
    <div class="row_bottom">
      <div class="card" v-for="card in arrayCardsBottom" :key="card.title">
        <div class="col_left">
          <h6>{{ card.calendar }}</h6>
          <h3>{{ card.title }}</h3>
          <small>{{ card.position }}</small>
        </div>
        <div class="col_right">
          <img :src="require('../assets/images/' + card.img)" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionOtto",
  data() {
    return {
      arrayCardsTop: [
        {
          img: "artist-event-04-250x300.jpg",
          calendar: "NOV 22, 2020",
          title: "Storytelling Workshop",
          position: "Texas, US",
        },
        {
          img: "artist-event-03-250x300.jpg",
          calendar: "OCT 10, 2020",
          title: "Paynting Art Contest 2020",
          position: "New York, US",
        },
      ],
      arrayCardsBottom: [
        {
          img: "artist-event-02-250x300.jpg",
          calendar: "NOV 23, 2020",
          title: "International Air Fair 2020",
          position: "Hamburg, Germany",
        },
        {
          img: "artist-event-01-250x300.jpg",
          calendar: "DEC 15, 2020",
          title: "Street Performance: Call for Artist",
          position: "Illinois, US",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.center {
  text-align: center;
  margin-top: 2rem;
  padding-top: 3rem;
  margin-bottom: 2rem;
}
h2 {
  margin-top: 1rem;
}
.row_top {
  display: flex;
  justify-content: center;
  margin-top: 1rem;
  margin-bottom: 4rem;
}
.row_bottom {
  display: flex;
  justify-content: center;
}
.row_bottom .card .col_left {
  text-align: end;
}
.card {
  display: flex;
  align-items: center;
  margin: 0 3rem;
}
img {
  margin: 0 1rem;
}
h3 {
  margin: 1rem 0;
}
h6,
small {
  color: gray;
}
</style>
