<template>
  <div id="charmander">
    <h2>Name: {{ charmander.name }}</h2>
    <p>type: {{ charmander.type }}</p>
    <p>number: {{ charmander.number }}</p>
    <p>ability: {{ charmander.ability }}</p>
  </div>
</template>

<script>
export default {
  name: "Charmander",
  data() {
    return {
      charmander: {
        name: "Charmander",
        type: "fire",
        number: "004",
        ability: "blaze"
      }
    }
  }
}
</script>

<style scoped>

</style>