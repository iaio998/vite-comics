<template>
  <div class="god">
    <div class="container h-100 position-relative">
      <button class="px-4">CURRENT SERIES</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppJumbo",
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;
.god {
  background-image: url(/img/jumbotron.jpg);
  background-size: cover;
  height: 400px;

  button {
    font-weight: bold;
    color: $color-white;
    background-color: $color-electric-blue;
    box-shadow: none;
    border: 0;
    padding: 10px;
    position: absolute;
    bottom: -25px;
    left: -1%;
    transition: 0.5s ease;

    &:hover {
      transform: scale(1.2);
    }
  }
}
</style>
