<template>
<section>
  <div class="container mt-5">
    <div class="row row-cols-2 row-cols-lg-5 g-2 g-lg-3 d-flex justify-content-between">
      <AppTrackCard />
      <AppTrackCard />
      <AppTrackCard />
      <AppTrackCard />
      <AppTrackCard />
    </div>
  </div>
</section>
</template>

<script>
import AppTrackCard from './AppTrackCard.vue';
import axios from 'axios';
export default {
    name: "AppTrackList",
    components: { AppTrackCard }
}
</script>

<style lang="scss" scoped>

</style>