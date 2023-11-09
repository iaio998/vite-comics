<script>
import App1Header from "./components/App1Header.vue";
import App2MainTop from "./components/App2MainTop.vue";
import App3MainBot from "./components/App3MainBot.vue";
import App4MainFooter from "./components/App4MainFooter.vue";
import App5Footer from "./components/App5Footer.vue";

export default {
  name: "App",
  components: {
    App1Header,
    App2MainTop,
    App3MainBot,
    App4MainFooter,
    App5Footer,
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
  <App4MainFooter />
  <App5Footer />
</template>

<style scoped></style>
