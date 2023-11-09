<script>
import App1Header from "./components/App1Header.vue";
import App2MainTop from "./components/App2MainTop.vue";
import App3MainBot from "./components/App3MainBot.vue";

export default {
  name: "App",
  components: {
    App1Header,
    App2MainTop,
    App3MainBot,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <App1Header />
  <App2MainTop />
  <App3MainBot />
</template>

<style scoped></style>
