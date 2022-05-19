<template>
  <header>
    <div class="logo">
      <img src="https://logos-world.net/wp-content/uploads/2020/09/Spotify-Symbol.png" alt="">
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader"
}
</script>

<style lang="scss" scoped>
@import "./style/variables.scss";
header {
  background-color: $bg-secondary-color;  
  .logo {
    width: 5rem;
    padding: 5px 0;
  }
}
</style>