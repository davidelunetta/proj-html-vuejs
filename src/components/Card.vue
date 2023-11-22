<template>
  <div class="d-flex flex-row justify-content-between align-items-center pe-5">
    <div v-for="item in myCard" class="my-card">
      <div class="logo">
        {{ item.logo }}
      </div>
      <div>
        <span class="title">
          {{ item.titolo }}
        </span>
        <div>
          <span class="description">{{ item.descrizione }}</span>
        </div>
      </div>
    </div>
  </div>

  <!-- AVADA NUMBER -->
  <div class="home d-flex justify-content-between align-items-center">
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-suitcase" style="color: #fed03d"></i>
      <span class="fw-2">3592</span>
      <span>PLANNING APPLICATIONS</span>
    </div>
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-building" style="color: #fed03d"></i>
      <span>896</span>
      <span>COMPLETED PROJECTS</span>
    </div>
    <div class="d-flex flex-column align-items-center">
      <i class="fa-solid fa-users" style="color: #fed03d"></i>
      <span>172</span>
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
    <a href="#"><button>VIEW ALL PROJECTS</button></a>
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
</template>

<script>
export default {
  name: "Card",
  data() {
    return {
      myCard: [
        {
          logo: '<i class="fa-solid fa-building"></i>',
          titolo: "Buildings",
          descrizione:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
          titoloRetro: "Artfully Crafted",
          testoRetro:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum.",
        },
        {
          logo: '<i class="fa-solid fa-rotate"></i>',
          titolo: "Renovate",
          descrizione:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
          titoloRetro: "Freshly New",
          testoRetro:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum.",
        },
        {
          logo: '<i class="fa-solid fa-house"></i>',
          titolo: "Construct",
          descrizione:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
          titoloRetro: "Perfect Lines",
          testoRetro:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum.",
        },
        {
          logo: '<i class="fa-solid fa-truck"></i>',
          titolo: "Exclusive",
          descrizione:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
          titoloRetro: "Planning",
          testoRetro:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/card.scss";
</style>
