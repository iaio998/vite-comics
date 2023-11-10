<script>
import Slide from "./Slide.vue";
export default {
  name: "App2MainTop",
  components: { Slide },
  data() {
    return {
      slides: [
        {
          image: "img/jumbotron.jpg",
          title: "Masked Mayhem",
          subtitle: "Batman squares off",
        },
        {
          image: "img/jumbotron.jpg",
          title: "Masked Elon",
          subtitle: "Batman squares off",
        },
        {
          image: "img/jumbotron.jpg",
          title: "Masked Pisello",
          subtitle: "Batman squares off",
        },
        {
          image: "img/jumbotron.jpg",
          title: "Pisell Elon ",
          subtitle: "Batman squares off",
        },
      ],
      indexSlide: 0,
    };
  },
  methods: {
    indexPlus() {
      this.indexSlide++;
    },
  },
};
</script>

<template>
  <div class="god">
    <div class="container">
      <p class="m-0 py-5 fs-3">CONTENT GOES HERE</p>
    </div>
    <!-- <Slide
      @click="indexPlus()"
      :img="slides[indexSlide].image"
      :title="slides[indexSlide].title"
      :subtitle="slides[indexSlide].subtitle"
    /> -->
  </div>
</template>

<style lang="css" scoped>
.god {
  background-color: black;
  color: white;
}
</style>
