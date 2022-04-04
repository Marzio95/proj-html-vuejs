<template>
  <footer>
    <div class="footer" id="footer">
      <div class="footer_container">
        <div class="col">
          <h3>Address</h3>
          <small>382 NE 191st ST # 87394 Miami, FL 33179-3899</small>
          <small>+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</small>
          <small>support@maxcoach.com</small>
          <small>icons</small>
        </div>

        <div class="col">
          <ul>
            <h3>Explore</h3>
            <li v-for="li in arrayUlOne" :key="li">
              <a href="#footer">{{ li }}</a>
            </li>
          </ul>
        </div>

        <div class="col">
          <ul>
            <h3>Information</h3>
            <li v-for="li in arrayUlTwo" :key="li">
              <a href="#footer">{{ li }}</a>
            </li>
          </ul>
        </div>

        <div class="col">
          <h3>Instagram <span>@maxcoach</span></h3>
          <div>
            <img src="../assets/images/old-man.jpg" alt="" />
            <img src="../assets/images/artist-event-03-250x300.jpg" alt="" />
            <img src="../assets/images/artist-event-02-250x300.jpg" alt="" />
          </div>
        </div>
      </div>
    </div>
    <div class="edits">
      <small class="credits"> 2020 Maxcoach, All Rights Reserved</small>
      <a class="up" href="#header">&#8593;</a>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterProj",
  data() {
    return {
      arrayUlOne: [
        "Start here",
        "Success story",
        "Blog",
        "Courses",
        "Contact us",
      ],
      arrayUlTwo: [
        "Membership",
        "Purchase guide",
        "Privacy policy",
        "Terms of services",
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.footer {
  min-height: 400px;
  display: flex;
  align-items: center;
}
.footer_container {
  width: 80%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}
.col {
  display: flex;
  flex-direction: column;
}
h3 {
  margin: 1rem 0;
}
small {
  color: gray;
  margin: 0.5rem 0;
}
ul {
  list-style: none;
}
li {
  color: gray;
  margin: 0.5rem 0;
}
img {
  width: 7rem;
  height: 7rem;
  margin-right: 0.5rem;
}
span {
  color: orangered;
}
.edits {
  margin: 2rem 0;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}
a {
  text-decoration: none;
  color: gray;
}
.up {
  position: absolute;
  right: 4rem;
  background-color: orangered;
  color: white;
  width: 4rem;
  height: 4rem;
  line-height: 3.6rem;
  border-radius: 50%;
  border: none;
  text-decoration: none;
  text-align: center;
  scroll-behavior: smooth;
  font-size: 2rem;
}
</style>
