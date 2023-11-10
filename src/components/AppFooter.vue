<script>
export default {
  name: "AppFooter",
  data() {
    return {
      links: [
        { id: 1, image: "img/footer-facebook.png" },
        { id: 2, image: "img/footer-twitter.png" },
        { id: 3, image: "img/footer-youtube.png" },
        { id: 4, image: "img/footer-pinterest.png" },
        { id: 5, image: "img/footer-periscope.png" },
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <div class="god w-100 d-flex align-items-center">
    <div class="container d-flex justify-content-between h-100">
      <div class="h-100 d-flex align-items-center">
        <button>SIGN UP NOW!</button>
      </div>
      <ul class="d-flex align-items-center m-0 p-0 gap-2">
        <h6 class="title m-0 px-2">FOLLOW US</h6>
        <li v-for="link in links">
          <a href="#"><img :src="link.image" alt="" /></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;
.god {
  background-color: #303030;
  color: white;
  height: 90px;
  position: fixed;
  z-index: 999;
  bottom: 0;
  right: 0;
}
.title {
  font-weight: bold;
  color: #0282f9;
}
button {
  font-weight: bold;
  color: white;
  background-color: transparent;
  box-shadow: none;
  border: 2px solid #0282f9;
  padding: 10px;
}
</style>
