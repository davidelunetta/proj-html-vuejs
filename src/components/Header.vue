<template>
  <div>
    <img src="../assets/img/construction_logo.png" alt="logo" />
    <nav class="">
      <ul class="">
       <li v-for="item in menuItems"><a href="#">{{ item }}</a></li>
      </ul>
    </nav>
  </div>
  <div id="hero" class="slider d-flex flex-column align-items-center">
    <h1>Building Inspiring Spaces</h1>
    <h5>We Build Inspiring Residential & Commercial Spaces</h5>
    <div>
      <button class="btn-header-right">Explore recent work</button>
      <button class="btn-header-left">Get a quote today</button>
    </div>
  </div>
  <div
    class="y-flag d-flex flex-column align-items-center justify-content-center"
  >
    <span class="pb-5"
      >Do you have a construction project we can help with?</span
    >
  </div>
  <div class="d-flex align-items-center justify-content-center ">
      <button>GET A FREE QUOTE</button>
  </div>
</template>

<script>
export default {
  name: "Header",

  data() {
    return {
      menuItems: ["Home", "About", "Services", "Contact"],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/main.scss";
</style>
