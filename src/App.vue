<template>
  <div class="app">
    <Header></Header>
    <Card></Card>
    <Main></Main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Card from "./components/Card.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
    Card,
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>
