<template>
  <div class="container">
    <div class="form-floating">
      <select
        class="form-select"
        id="floatingSelect"
        aria-label="Floating label select example"
        v-model="filterGenre"
        @change="sendEvent"
      >
        <option selected>Tutti i generi</option>
        <option value="rock">Rock</option>
        <option value="jazz">Jazz</option>
        <option value="pop">Pop</option>
        <option value="metal">Metal</option>
      </select>
      <label for="floatingSelect">Filtra per genere</label>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFilter",
  data: function() {
    return {
      filterGenre: ""
    };
  },
  methods: {
    sendEvent() {
      this.$emit("selectedGenre", this.filterGenre)
    }
  }
};
</script>

<style>
</style>