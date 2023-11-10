<script>
export default {
  name: "App4MainFooter",
  data() {
    return {
      first: [
        "Characters",
        "Comics",
        "Movies",
        "Tv",
        "Games",
        "Videos",
        "News",
      ],
      second: ["Shop DC", "Shop DC Collectibles"],
      third: [
        "Terms of Use",
        "Privacy Policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      fourth: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
    };
  },
  methods: {},
};
</script>

<template>
  <div class="god py-4">
    <div class="container d-flex justify-content-between">
      <div class="d-flex">
        <div>
          <ul class="p-0">
            <h4>DC COMICS</h4>
            <li v-for="element in first">
              <a href="#">{{ element }}</a>
            </li>
          </ul>
          <ul class="p-0">
            <h4>SHOP</h4>
            <li v-for="element in second">
              <a href="#">{{ element }}</a>
            </li>
          </ul>
        </div>
        <div class="d-flex">
          <ul>
            <h4>DC</h4>
            <li v-for="element in third">
              <a href="#">{{ element }}</a>
            </li>
          </ul>
          <ul>
            <h4>SITES</h4>
            <li v-for="element in fourth">
              <a href="#">{{ element }}</a>
            </li>
          </ul>
        </div>
      </div>
      <div>
        <img id="logo-bg" src="/img/dc-logo-bg.png" alt="Logo background" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;
.god {
  background-image: url(/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  color: white;
  height: 500px;
}
a {
  color: #91918f;
}
#logo-bg {
  width: 500px;
  height: 500px;
  transform: translate(0, -10%);
}
</style>
