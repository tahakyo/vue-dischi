<template>
  <div class="track-card text-center">
    <img :src="albumObj.poster" alt="">
    <h2 class="fw-bold fs-5 text-uppercase">{{albumObj.title}}</h2>
    <h5>{{albumObj.author}}</h5>
    <h6>{{albumObj.year}}</h6>
  </div>
</template>

<script>
export default {
  name: "AppTrackCard",
  props: {
    albumObj: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "./style/variables.scss";
.track-card {
  height: 375px;
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