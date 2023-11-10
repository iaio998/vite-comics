<script>
import Card from "./Card.vue";
import { cards } from "../assets/data/data.js";

export default {
  name: "App2MainTop",
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
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;
.god {
  background-color: $color-black;
  color: white;
}
</style>
