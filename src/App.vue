<template>
  <div id="app">
    <header>
      <AppHeader />
    </header>
    <main>
      <AppTrackList />
      <AppTrackCard />
    </main>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppTrackList from './components/AppTrackList.vue';
import AppTrackCard from './components/AppTrackCard.vue';
export default {
  name: 'App',
  components: {
    AppHeader,
    AppTrackList,
    AppTrackCard,
}
}
</script>

<style lang="scss">
@import "./components/style/common.scss";
</style>
