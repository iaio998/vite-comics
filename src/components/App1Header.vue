<template>
  <div class="god">
    <nav class="container d-flex align-items-center justify-content-between">
      <span>
        <img src="/public/img/dc-logo.png" alt="Logo" />
      </span>
      <ul class="d-flex">
        <li class=""><a href="#">1</a></li>
        <li><a href="#">2</a></li>
        <li><a href="#">3</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "App1Header",
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="css" scoped>
.god {
  background-color: white;
  color: black;
}
a {
  color: black;
}
</style>
