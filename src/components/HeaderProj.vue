<template>
  <header>
    <div class="header_time" id="header">
      <div class="starts">
        Starts TOMORROW! Our biggest event of the year...
      </div>
      <div id="timer"></div>
      <button class="ticket">Get ticket</button>
    </div>
    <nav class="navbar">
      <img class="logo" src="../assets/images/dark-logo.png" alt="Logo" />
      <ul class="list_nav">
        <li v-for="element in arrayNav" :key="element">
          <a href="#">{{ element }}</a>
        </li>
      </ul>
      <div class="icon_flex">
        <font-awesome-icon icon="fa-brands fa-twitter" />
        <font-awesome-icon icon="fa-brands fa-facebook-f" />
        <font-awesome-icon icon="fa-brands fa-instagram" />
        <font-awesome-icon icon="fa-brands fa-linkedin" />
      </div>
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

  created() {
    // Set the date we're counting down to
    var countDownDate = new Date("jun 10, 2022 23:59:59").getTime();

    // Update the count down every 1 second
    var x = setInterval(function () {
      // Get today's date and time
      var now = new Date().getTime();

      // Find the distance between now and the count down date
      var distance = countDownDate - now;

      // Time calculations for days, hours, minutes and seconds
      var days = Math.floor(distance / (1000 * 60 * 60 * 24));
      var hours = Math.floor(
        (distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60)
      );
      var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      var seconds = Math.floor((distance % (1000 * 60)) / 1000);

      // Output the result in an element with id="demo"
      document.querySelector("#timer").innerHTML =
        days + " D : " + hours + " H : " + minutes + " M : " + seconds + " S";

      // If the count down is over, write some text
      if (distance < 0) {
        clearInterval(x);
        document.querySelector("#timer").innerHTML = "EXPIRED";
      }
    }, 1000);
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
#timer {
  font-weight: 700;
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
.icon_flex {
  display: flex;
  gap: 1rem;
  color: gray;
}
</style>
