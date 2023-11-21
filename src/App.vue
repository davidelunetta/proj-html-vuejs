<template>
  <div class="app">
    <Header></Header>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
// import { store } from "../src/assets/data/store.js";
export default {
  name: "App",
  components: {
    Header,
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>
