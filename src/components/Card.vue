<template>
  <div
    class="pt-5 pb-5 d-flex flex-column justify-content-center align-items-center text-center"
  >
    <span class="fw-medium fs-3"> Specialists in modern construction </span>
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
  <div
    class="d-flex flex-row justify-content-between align-items-center ps-5 pe-5"
  >
    <div
      v-for="(item, index) in myCard"
      @mouseover="showRetro(index)"
      @mouseout="hideRetro(index)"
      :key="index"
      class="my-card card-construction"
    >
      <div class="card-content">
        <div class="normal-state">
          <div class="d-flex align-items-center justify-content-center">
            <div
              class="logo d-flex align-items-center justify-content-center fs-3"
              v-html="item.logo"
            ></div>
          </div>

          <h3>{{ item.titolo }}</h3>
          <p>{{ item.descrizione }}</p>
        </div>
        <div class="hover-state" v-show="item.showRetro">
          <h3>{{ item.titoloRetro }}</h3>
          <p>{{ item.testoRetro }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  methods: {
    showRetro(index) {
      this.myCard[index].showRetro = true;
    },
    hideRetro(index) {
      this.myCard[index].showRetro = false;
    },
  },
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
          showRetro: false,
        },
        {
          logo: '<i class="fa-solid fa-rotate"></i>',
          titolo: "Renovate",
          descrizione:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
          titoloRetro: "Freshly New",
          testoRetro:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum.",
          showRetro: false,
        },
        {
          logo: '<i class="fa-solid fa-house"></i>',
          titolo: "Construct",
          descrizione:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
          titoloRetro: "Perfect Lines",
          testoRetro:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum.",
          showRetro: false,
        },
        {
          logo: '<i class="fa-solid fa-truck"></i>',
          titolo: "Exclusive",
          descrizione:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
          titoloRetro: "Planning",
          testoRetro:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum.",
          showRetro: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/card.scss";
.normal-state {
  display: block;
}

.hover-state {
  display: none;
}

.my-card:hover .normal-state {
  display: none;
}

.my-card:hover .hover-state {
  display: block;
}
</style>
