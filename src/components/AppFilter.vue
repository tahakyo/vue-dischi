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
        <option selected value="">Tutti i generi</option>
        <option value="Rock">Rock</option>
        <option value="Jazz">Jazz</option>
        <option value="Pop">Pop</option>
        <option value="Metal">Metal</option>
      </select>
      <label for="floatingSelect">Filtra per genere</label>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFilter",
  data: function () {
    return {
      filterGenre: "",
    };
  },
  methods: {
    sendEvent() {
      this.$emit("selectedGenre", this.filterGenre);
    },
  },
};
</script>

<style>
</style>