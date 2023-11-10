<script>
import Card from "./sons/Card.vue";
import { cards } from "../assets/data/data.js";

export default {
  name: "AppMainTop",
  components: { Card },
  data() {
    return {
      comics: cards,
    };
  },
  methods: {},
};
</script>

<template>
  <div class="god">
    <div class="container py-5">
      <div class="row g-2">
        <Card v-for="el in comics" :img="el.thumb" :title="el.series" />
      </div>
      <div class="d-flex justify-content-center">
        <button class="my-2">LOAD MORE</button>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;
.god {
  background-color: $color-black;
  color: white;

  button {
    margin: 0 auto;
    font-weight: bold;
    color: $color-white;
    background-color: $color-electric-blue;
    box-shadow: none;
    border: 0;
    padding: 10px 50px;

    &:hover {
      transform: scale(1.2);
    }
  }
}
</style>
