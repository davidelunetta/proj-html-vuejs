<template>
  <div class="d-flex justify-content-between">
    <div>
      <img src="../assets/img/construction_logo.png" alt="logo" />
    </div>
    <div class="d-flex flex-row">
      <nav class="pe-5">
        <ul class="d-flex mt-4">
          <li v-for="item in menuItems">
            <a class="me-5 fs-5" href="#">{{ item }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
  <div
    id="hero"
    class="slider d-flex flex-column align-items-center justify-content-center"
  >
    <h1>Building Inspiring Spaces</h1>
    <h5 class="pt-3">We Build Inspiring Residential & Commercial Spaces</h5>
    <div class="pt-3">
      <button class="btn-header-left">Explore recent work</button>
      <button class="btn-header-right">Get a quote today</button>
    </div>
  </div>
  <div
    class="y-flag d-flex flex-column align-items-center justify-content-center"
  >
    <span class="pb-5"
      >Do you have a construction project we can help with?</span
    >
  </div>
  <div class="d-flex align-items-center justify-content-center">
    <button class="btn-header-left">GET A FREE QUOTE</button>
  </div>
</template>

<script>
export default {
  name: "Header",

  data() {
    return {
      menuItems: ["Home", "About", "Services", "Work", "Articles", "Get Quote"],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/main.scss";
</style>
