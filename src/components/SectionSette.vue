<template>
  <section>
    <div class="center">
      <div class="particular_text">Articles and Tips</div>
      <h2>Latest From The Blog</h2>
    </div>
    <div class="flex">
      <div class="circle"></div>
      <div class="container_img">
        <div class="container_text">
          <h5>ARTIST</h5>
          <h2>Connection Between Self- <br />Portrais ind Identity</h2>
          <small>May 15, 2020 <span>397 views</span></small>
        </div>
      </div>
      <div class="card" v-for="card in arrayCards" :key="card.texts">
        <img :src="require('../assets/images/' + card.img)" alt="" />
        <div class="card_text">
          <div>{{ card.artist }}</div>
          <h3>{{ card.text }}</h3>
          <small
            ><font-awesome-icon class="icon" icon="fa-regular fa-calendar" />
            {{ card.calendar }}
            <font-awesome-icon class="icon_right" icon="fa-regular fa-eye" />{{
              card.views
            }}</small
          >
        </div>
      </div>
    </div>
    <div class="text_center">
      Get into details now? <a href="#">View all posts</a>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionSette",
  data() {
    return {
      arrayCards: [
        {
          img: "old-man.jpg",
          artist: "ARTIST",
          text: "Brush Strokes Energize Trees in Paintings",
          calendar: "May15, 2020",
          views: "688 views",
        },
        {
          img: "artist-blog-01-480x356.jpg",
          artist: "ARTIST",
          text: "Pocket-Sized Notebooks Hold Miniature Paintings",
          calendar: "May15, 2020",
          views: "603 views",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
section {
  background-color: #f4f0ef;
  height: 1020px;
}
.center {
  text-align: center;
  margin-top: 4rem;
  padding-top: 4rem;
  margin-bottom: 2rem;
}
.container_img {
  background-image: url(../assets/images/artist-blog-02-500x680.jpg);
  height: 600px;
  width: 500px;
  padding: 3rem;
  filter: brightness(0.8);
  justify-self: center;
  margin-left: 11rem;
}
.container_text {
  color: white;
  margin-top: 23rem;
}
.flex {
  display: flex;
  justify-content: center;
  width: 100%;
  background-image: url(../assets/images/maxcoach-shape-03.png);
  background-position-y: top;
}
h2 {
  font-size: 2rem;
  margin: 1rem 0;
}
img {
  width: 260px;
  height: 230px;
}
.card {
  background-color: white;
  height: 400px;
  width: 260px;
  position: absolute;
  left: 5rem;
  margin-top: 5rem;
}
.card_text {
  padding: 1rem;
}
h3 {
  margin: 1rem 0;
}
.card:last-child {
  position: relative;
  right: 6rem;
  margin-top: 0;
}
.circle {
  width: 5rem;
  height: 5rem;
  border: 8px solid orange;
  border-radius: 50%;
  margin-top: -3rem;
}
.text_center {
  padding-top: 5rem;
  text-align: center;
  font-size: 1.5rem;
}
a {
  color: orangered;
  font-weight: 600;
  text-decoration: none;
}
.icon {
  margin-right: 0.4rem;
}
.icon_right {
  margin-left: 1rem;
  margin-right: 0.7rem;
}
</style>
