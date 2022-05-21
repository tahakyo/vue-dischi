<template>
  <div class="container">
    <div class="form-floating">
      <select
        class="form-select"
        id="floatingSelect"
        aria-label="Floating label select example"
      >
        <option selected>Clicca per selezionare</option>
        <option value="1">Rock</option>
        <option value="2">Jazz</option>
        <option value="3">Pop</option>
        <option value="4">Metal</option>
      </select>
      <label for="floatingSelect">Filtra per genere</label>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFilter",
};
</script>

<style>
</style>