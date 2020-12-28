<template>
  <div id="Pokemon">
    <h2>Name: {{ details.name }}</h2>
    <p>type: {{ details.type }}</p>
  </div>
</template>

<script>
export default {
  name: "Pokemon",
  props: {
    details: {
      type: Object,
      default: () => {
        return { name: "", type: ""};
      },
    },
  },
  data() {
    return {};
  },
};
</script>

<style scoped>

</style>