<script>
import AppHeader from "./components/AppHeader.vue";
import AppJumbo from "./components/AppJumbo.vue";
import AppMainTop from "./components/AppMainTop.vue";
import AppMainBot from "./components/AppMainBot.vue";
import AppMainFooter from "./components/AppMainFooter.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppJumbo,
    AppMainTop,
    AppMainBot,
    AppMainFooter,
    AppFooter,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <AppHeader />
  <AppJumbo />
  <AppMainTop />
  <AppMainBot />
  <AppMainFooter />
  <AppFooter />
</template>

<style scoped></style>
