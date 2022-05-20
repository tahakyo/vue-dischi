<template>
  <div id="app">
    <header>
      <AppHeader />
    </header>
    <main>
      <AppTrackList />
    </main>
    <footer></footer>
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
</style>
