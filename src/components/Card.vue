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
    <div><i class="fa-solid fa-suitcase" style="color: #fed03d"></i></div>
    <div>b</div>
    <div>c</div>
    <div>d</div>
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
