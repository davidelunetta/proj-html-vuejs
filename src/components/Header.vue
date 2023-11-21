<template>
  <div>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </div>
  <div id="hero" class="container">
    <img src="../assets/img/home-slider-62528242.jpg" alt="slider" />
    <h1>Building Inspiring Spaces</h1>
    <h5>We Build Inspiring Residential & Commercial Spaces</h5>
    <button>Explore recent work</button>
    <button>Get a quote today</button>
  </div>
  <div class="container d-flex">
    <span>Do you have a construction project we can help with?</span>
    <button>GET A FREE QUOTE</button>
  </div>
</template>

<script>
export default {
  name: "Header",

  data() {
    return {
      store,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/main.scss";
</style>
