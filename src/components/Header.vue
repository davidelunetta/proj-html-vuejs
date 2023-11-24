<template>
  <div
    class="my-nav d-flex justify-content-between align-items-center bg-white px-5"
  >
    <div class="ms-4">
      <img src="../assets/img/construction_logo.png" alt="logo" />
    </div>
    <div class="d-flex flex-row">
      <nav class="pe-5">
        <ul class="d-flex mt-4">
          <li
            v-for="(item, index) in menuItems"
            class="d-flex align-items-center"
          >
            <a
              :class="{
                'me-5': index < menuItems.length - 1,
                'me-0 px-4 py-2 nav-link ': index === menuItems.length - 1,
                'fs-5  ': true,
              }"
              href="#"
              >{{ item }}</a
            >
          </li>
        </ul>
      </nav>
    </div>
  </div>
  <div id="navBarPlaceHolder"></div>
  <div
    id="hero"
    class="slider d-flex flex-column align-items-center justify-content-center"
  >
    <h1>Building Inspiring Spaces</h1>
    <h5 class="pt-3">We Build Inspiring Residential & Commercial Spaces</h5>
    <div class="pt-3">
      <button class="btn-header-left me-1 fw-semibold">
        EXPLORE RECENT WORK
      </button>
      <button class="btn-header-right ms-1 fw-semibold">
        GET A QUOTE TODAY
      </button>
    </div>
  </div>
  <div
    class="y-flag d-flex flex-column align-items-center justify-content-center mb-4"
  >
    <span class="">Do you have a construction project we can help with?</span>
    <div class="quote-btn d-flex align-items-center justify-content-center">
      <button class="btn-header-left">GET A FREE QUOTE</button>
    </div>
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
.nav-link {
  background-color: #fed03d;
}
</style>
