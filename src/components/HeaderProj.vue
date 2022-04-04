<template>
  <header>
    <div class="header_time" id="header">
      <div class="starts">
        Starts TOMORROW! Our biggest event of the year...
      </div>
      <div class="timer">00 : 00 : 00 : 00</div>
      <button class="ticket">Get ticket</button>
    </div>
    <nav class="navbar">
      <img class="logo" src="../assets/images/dark-logo.png" alt="Logo" />
      <ul class="list_nav">
        <li v-for="element in arrayNav" :key="element">
          <a href="#">{{ element }}</a>
        </li>
      </ul>
      <div>icones</div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "HeaderProj",
  data() {
    return {
      arrayNav: ["Home", "Pages", "Courses", "Features", "Blog", "Shop"],
    };
  },
};
</script>

<style scoped lang="scss">
.header_time {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 3.5rem;
  background-color: #f4f0ef;
}
.starts {
  color: gray;
  margin-left: 4rem;
  font-size: 0.9rem;
}
.timer {
  font-weight: 800;
  margin-left: 2rem;
  margin-right: 4rem;
}
.ticket {
  padding: 0.5rem;
  color: white;
  border: none;
  border-radius: 7px;
  font-weight: 600;
  background-color: #ec601c;
  width: 10rem;
}
.ticket:hover {
  background-color: #b1e4f4;
}
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  min-height: 5rem;
  width: 80%;
  margin: auto;
}
.logo {
  height: 1.7rem;
}
.list_nav {
  list-style: none;
}
li {
  display: inline-block;
  margin: 0 0.8rem;
}
</style>
