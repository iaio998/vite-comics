<template>
  <div>
    <h2>{{ title }}</h2>
    <img :src="img" alt="" />
    <h5>{{ subtitle }}</h5>
  </div>
</template>

<script>
export default {
  name: "Slide",
  props: {
    img: String,
    title: String,
    subtitle: String,
  },
};
</script>

<style lang="css" scoped>
img {
  width: 350px;
  height: 150px;
}
</style>
