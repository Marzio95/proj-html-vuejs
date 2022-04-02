<template>
  <div class="center_main">
    <img src="../assets/images/artist-video-poster.jpg" alt="" />
    <img class="center" src="../assets/images/icon-youtube-play.png" alt="" />
    <img class="right" src="../assets/images/maxcoach-shape-12.png" alt="" />
    <img class="left" src="../assets/images/maxcoach-shape-12.png" alt="" />
  </div>
</template>

<script>
export default {
  name: "SectionQuattro",
};
</script>

<style scoped lang="scss">
.center_main {
  text-align: center;
  position: relative;
}
.center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.right {
  position: absolute;
  right: 10rem;
  bottom: 0;
  z-index: -1;
}
.left {
  position: absolute;
  top: 0;
  left: 10rem;
  z-index: -1;
}
</style>
