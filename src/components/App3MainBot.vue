<template>
  <div class="god">
    <div class="container">
      <div class="row d-flex m-0 g-5 py-4">
        <div class="col m-0 p-0" v-for="(option, index) in menu">
          <a href="#"
            ><img :src="option.img" :alt="option.text" /> {{ option.text }}</a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App3MainBot",
  data() {
    return {
      menu: [
        {
          id: 1,
          text: "DIGITAL COMICS",
          img: "img/buy-comics-digital-comics.png",
        },
        {
          id: 2,
          text: "DC MERCHANDASING",
          img: "img/buy-comics-merchandise.png",
        },
        {
          id: 3,
          text: "SUBSCRIPTION",
          img: "img/buy-comics-shop-locator.png",
        },
        {
          id: 4,
          text: "COMIC SHOP LOCATOR",
          img: "img/buy-comics-subscriptions.png",
        },
        {
          id: 5,
          text: "DC POWER VISA",
          img: "img/buy-dc-power-visa.svg",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style lang="css" scoped>
.god {
  background-color: #0282f9;
  color: white;
}
a {
  color: white;
}
img {
  width: 50px;
  height: 50px;
  /* display: block; */
}
span {
}
</style>
