<template>
  <b-container class="p-3 bg-secondary home-view rounded">
    <b-row>
      <div id="blue-ball" class="bg-primary rounded-circle m-4"/>
      <div class="tiny-balls bg-danger rounded-circle mr-1 mt-4"/>
      <div class="tiny-balls bg-warning rounded-circle mr-1 mt-4"/>
      <div class="tiny-balls bg-success rounded-circle mr-1 mt-4"/>

      <p>Hello {{ name }}</p>
    </b-row>
    <b-row>
      <div id="app">
        <Pokemon :details="charmander"/>
        <Pokemon :details="bulbasaur"/>
        <Pokemon :details="squirtle"/>
      </div>
    </b-row>
    <b-row>
    </b-row>
  </b-container>
</template>

<script>
import Pokemon from "@/components/Pokemon";

export default {
  name: "Home",
  components: {
    Pokemon
  },
  data() {
    return {
      charmander: {
        name: "Charmander",
        type: "fire",
      },
      bulbasaur: {
        name: "Bulbasaur",
        type: "grass",
      },
      squirtle: {
        name: "Squirtle",
        type: "water",
      },
      name: "Muriel",
      components: {
        Pokemon,
      },
    };
  },
  computed: {
  },
  methods: {
  }
};
</script>

<style lang="scss">
#blue-ball {
  height: 70px;
  width: 70px;
  border: 10px solid lightgrey;
}

.tiny-balls {
  height: 20px;
  width: 20px;
  border: 1px solid black;
}

.home-view {
  border: 3px solid black;
}
</style>