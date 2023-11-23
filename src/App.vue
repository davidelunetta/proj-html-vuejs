<template>
  <div class="app">
    <Header></Header>
    <Card></Card>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Card from "./components/Card.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
    Card,
    Footer,
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>
