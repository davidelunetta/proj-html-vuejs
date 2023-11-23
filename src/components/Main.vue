<template>
  <!-- AVADA NUMBER -->
  <div class="home d-flex justify-content-between align-items-center">
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-suitcase fa-2xl" style="color: #fed03d"></i>
      <span class="mt-4">3592</span>
      <span>PLANNING APPLICATIONS</span>
    </div>
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-building fa-2xl" style="color: #fed03d"></i>
      <span class="mt-4">896</span>
      <span>COMPLETED PROJECTS</span>
    </div>
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-users fa-2xl" style="color: #fed03d"></i>
      <span class="mt-4">172</span>
      <span>TRAINED PROFESSIONALS</span>
    </div>
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-globe fa-2xl" style="color: #fed03d"></i>
      <span class="mt-4">19</span>
      <span>INTERNATIONALS OFFICES</span>
    </div>
  </div>
  <div
    class="pt-5 pb-5 d-flex flex-column justify-content-center align-items-center text-center"
  >
    <span class="fw-medium fs-3"> Explore recent works </span>
    <div class="separator mt-3"></div>
    <div class="container mt-3">
      <span class="text-center"
        >Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum
        distinctio doloribus quidem odio, ipsum hic facere nesciunt consequuntur
        laudantium corrupti explicabo recusandae aut consequatur nam magnam
        doloremque architecto enim magni.
      </span>
    </div>
  </div>
  <div class="recent-works d-flex justify-content-between">
    <div>
      <img
        src="../assets/img/project2-featured-15013609-400x400.jpg"
        alt="project2"
      />
    </div>
    <div>
      <img
        src="../assets/img/project1-featured-294276386-400x400.jpg"
        alt="project1"
      />
    </div>
    <div>
      <img
        src="../assets/img/project3-featured-189023420-400x400.jpg"
        alt="project3"
      />
    </div>
  </div>
  <div class="d-flex justify-content-between mt-5">
    <div class="line ms-5 mt-3"></div>
    <a href="#"><button class="btn-projects">VIEW ALL PROJECTS</button></a>
    <div class="line me-5 mt-3"></div>
  </div>
  <div
    class="pt-5 pb-5 d-flex flex-column justify-content-center align-items-center text-center"
  >
    <span class="fw-medium fs-3"> Our Core Values </span>
    <div class="separator mt-3"></div>
    <div class="container mt-3">
      <span class="text-center"
        >Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum
        distinctio doloribus quidem odio, ipsum hic facere nesciunt consequuntur
        laudantium corrupti explicabo recusandae aut consequatur nam magnam
        doloremque architecto enim magni.
      </span>
    </div>
  </div>

  <div class="d-flex justify-content-between mt-3 ms-5">
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-house"></i>
      <span>Great Services</span>
      <div class="grey-line"></div>
      <span class="text-center"
        >Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet,
        consectetur, adipisci velit, sed quia</span
      >
    </div>
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-house"></i>
      <span>Great Services</span>
      <div class="grey-line"></div>
      <span class="text-center"
        >Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet,
        consectetur, adipisci velit, sed quia</span
      >
    </div>
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-house"></i>
      <span>Great Services</span>
      <div class="grey-line"></div>
      <span class="text-center"
        >Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet,
        consectetur, adipisci velit, sed quia</span
      >
    </div>
    <div class="d-flex flex-column align-items-center me-5">
      <i class="fa-solid fa-house"></i>
      <span>Great Services</span>
      <div class="grey-line"></div>
      <span class="text-center"
        >Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet,
        consectetur, adipisci velit, sed quia</span
      >
    </div>
  </div>
  <div
    class="parallax d-flex flex-column justify-content-center align-items-center"
  >
    <span class="fw-medium fs-3"> Our Home Owners Say </span>
    <div class="separator mt-3"></div>
    <div class="tab-container">
      <div
        v-for="(tab, index) in tabs"
        :key="index"
        class="tab-content"
        :class="{ active: activeTab === index }"
      >
        <div class="d-flex flex-column justify-content-center">
          <img :src="tab.image" alt="img" class="tab-image mt-3" />
          <span>{{ tab.content }}</span>
        </div>
      </div>
    </div>
    <div class="tabs">
      <button
        v-for="(tab, index) in tabs"
        :key="index"
        @click="activateTab(index)"
        :class="{ active: activeTab === index }"
      ></button>
    </div>
  </div>
  <div
    class="pt-5 pb-5 d-flex flex-column justify-content-center align-items-center text-center"
  >
    <span class="fw-medium fs-3"> Latest News </span>
    <div class="separator mt-3"></div>
    <div class="container mt-3">
      <span class="text-center"
        >Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum
        distinctio doloribus quidem odio, ipsum hic facere nesciunt consequuntur
        laudantium corrupti explicabo recusandae aut consequatur nam magnam
        doloremque architecto enim magni.
      </span>
    </div>
  </div>
  <div class="container">
    <div class="d-flex justify-content-between align-items-center">
      <div v-for="(item, index) in items" :key="index" class="card-news">
        <div class="text-center mx-2">
          <img
            :src="item.image"
            :alt="item.title"
            style="width: 350px; height: 200px"
          />
        </div>
        <div class="ps-3 pe-3 d-flex flex-column">
          <h2 class="">
            <a :href="item.link">{{ item.title }}</a>
          </h2>
          <small class="text-gray">{{ item.date }}</small>
          <span class="">{{ item.paragraph }}</span>
        </div>
      </div>
    </div>
  </div>
  <div class="d-flex justify-content-between mt-5">
    <div class="line ms-5 mt-3"></div>
    <a href="#"><button class="btn-projects">VIEW ALL ARTICLES</button></a>
    <div class="line me-5 mt-3"></div>
  </div>
  <div
    class="pt-5 pb-5 d-flex flex-column justify-content-center align-items-center text-center"
  >
    <span class="fw-medium fs-3"> Trusted Partners </span>
    <div class="separator mt-3"></div>
    <div class="container mt-3">
      <span class="text-center"
        >Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum
        distinctio doloribus quidem odio, ipsum hic facere nesciunt consequuntur
        laudantium corrupti explicabo recusandae aut consequatur nam magnam
        doloremque architecto enim magni.
      </span>
    </div>
  </div>
  <!-- CAROUSEL -->
  <div class="my-container pb-5">
    <split-carousel>
      <split-carousel-item v-for="image in images" :key="image.id">
        <img :src="image.src" :alt="image.alt" />
      </split-carousel-item>
    </split-carousel>
  </div>
</template>

<script>
import { SplitCarousel, SplitCarouselItem } from "vue-split-carousel";
export default {
  name: "Main",
  components: {
    SplitCarousel,
    SplitCarouselItem,
  },

  data() {
    return {
      activeTab: 0,
      tabs: [
        {
          image: "./src/assets/img/home-testimonial-84268399.jpg",
          content:
            "“Many novice real estate investors soon quit the profession and invest. When you invest in real estate, you often see a side of humanity that stocks, bonds, mutual funds, and saving money shelter you from.”",
        },
        {
          image: "./src/assets/img/home-testimonial-113165296.jpg",
          content: "Contenuto del Tab 2",
        },
      ],
      items: [
        {
          image: "/src/assets/img/blog-post-134132600-1200x723.jpg",
          title: "Redeveloping Florida’s Remote Southern Coast",
          link: "https://link1.com",
          date: "December 7th, 2015",
          paragraph:
            "Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed",
        },
        {
          image: "/src/assets/img/blog-post-92486644-1200x723.jpg",
          title: "How We Manage Large Construction Projects",
          link: "https://link2.com",
          date: "December 7th, 2015",
          paragraph:
            "Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed",
        },
        {
          image: "/src/assets/img/blog-post-332773904-1200x723.jpg",
          title: "Future proofing a modern home",
          link: "https://link3.com",
          date: "December 6th, 2015",
          paragraph:
            "Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed",
        },
      ],
      images: [
        {
          id: 1,
          src: "/src/assets/img/home-logo1-219096700-320x202.png",
          alt: "Partner 1",
        },
        {
          id: 2,
          src: "/src/assets/img/home-logo2-219096700-320x202.png",
          alt: "Partner 2",
        },
        {
          id: 3,
          src: "/src/assets/img/home-logo9-219096700-320x202.png",
          alt: "Partner 3",
        },
        {
          id: 4,
          src: "/src/assets/img/home-logo10-219096700-320x202.png",
          alt: "Partner 4",
        },
        {
          id: 5,
          src: "/src/assets/img/home-logo11-219096700-320x202.png",
          alt: "Partner 5",
        },
      ],
    };
  },

  mounted() {
    setInterval(() => {
      this.activeTab = (this.activeTab + 1) % this.tabs.length;
    }, 10000);
  },
  methods: {
    activateTab(index) {
      this.activeTab = index;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/main.scss";
</style>
