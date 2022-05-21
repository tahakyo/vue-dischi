<template>
  <div id="app">
    <!-- Header -->
    <header>
      <AppHeader />
    </header>
    <!-- Header -->
    <!-- Main -->
    <main>
      <AppTrackList />
    </main>
    <!-- Main -->
    <!-- Footer -->
    <footer></footer>
    <!-- Footer -->
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppTrackList from './components/AppTrackList.vue';
export default {
  name: 'App',
  components: {
    AppHeader,
    AppTrackList,
  }
}
</script>

<style lang="scss">
@import "./components/style/common.scss";
main {
  height: 1200px;
}
</style>
