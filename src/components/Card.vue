<template>
  <div class="col-2">
    <div class="">
      <img :src="img" class="" :alt="title" />
      <div class="">
        <h5 class="title">{{ title }}</h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    img: String,
    price: String,
    title: String,
    subtitle: String,
  },
};
</script>

<style lang="css" scoped>
img {
  width: 200px;
  height: 200px;
}
.title {
  width: 90%;
  padding: 5px 0;
}
</style>
