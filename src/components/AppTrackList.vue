<template>
  <section>
    <AppFilter />
    <div class="container ms_container mt-5">
      <div
        class="
          row row-cols-2 row-cols-md-5 row-cols-lg-5
          g-2 g-lg-3
          d-flex
          justify-content-between
          flex-wrap
        "
      >
        <AppTrackCard
          v-for="(item, index) in trackList"
          :key="index"
          :albumObj="item"
        />
      </div>
    </div>
  </section>
</template>

<script>
import AppTrackCard from "./AppTrackCard.vue";
import axios from "axios";
import AppFilter from "./AppFilter.vue";
export default {
  name: "AppTrackList",
  components: {
    AppTrackCard,
    AppFilter
},
  data: function () {
    return {
      trackList: [],
    };
  },
  created() {
    axios
      .get("https://flynn.boolean.careers/exercises/api/array/music")
      .then((resp) => {
        this.trackList = resp.data.response;
      });
  },
};
</script>

<style lang="scss" scoped>
.ms_container {
  max-width: 1200px;
  max-height: 750px;
  overflow: auto;
}
</style>