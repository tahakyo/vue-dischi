<template>
  <div class="track-card text-center">
    <img src="https://img.discogs.com/vknPDdrqRbT92pNRX0W4I5N91jg=/fit-in/300x300/filters:strip_icc():format(jpeg):mode_rgb():quality(40)/discogs-images/R-1246953-1448927086-6590.jpeg.jpg" alt="">
    <h2 class="fw-bold fs-5 text-uppercase">Live at Wembley 86</h2>
    <h5>Queen</h5>
    <h6>1992</h6>
  </div>
</template>

<script>
export default {
  name: "AppTrackCard"
}
</script>

<style lang="scss" scoped>
@import "./style/variables.scss";
.track-card {
  height: 360px;
  width: 200px;
  background-color: $bg-secondary-color;
  padding: 1rem;
  h2 {
    color: white;
    padding: 1rem
  }
  h5 {
    color: $small-title-color;
  }
  h6 {
    color: $small-title-color;
  }
}
</style>