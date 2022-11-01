<template>
  <header>
    <div class="logo-nav">
      <img src="../assets/image/image1.png" alt="logo" class="logo-img" />
    </div>
    <div class="nav-link">
      <div class="hamber-menu" @click="opeenNav">
        <img
          src="../assets/image/icon/icons8-menu-rounded-50.png"
          alt=""
          width="30"
        />
      </div>
      <div class="nav-bar" v-if="closes">
        <img src="../assets/image/image1.png" alt="logo" class="logo-img1" />
        <div v-for="link in linkNav" :key="link.path" class="">
          <div class="div-navItem">
            <router-link :to="link.path" class="nav-item1">{{
              link.name
            }}</router-link>
          </div>
        </div>
        <div class="close-side" @click="close">
          <img
            src="../assets/image/icon/icons8-back-arrow-50.png"
            alt=""
            width="30"
          />
        </div>
      </div>
      <div v-for="link in linkNav" :key="link.path" class="div-item">
        <router-link :to="link.path" class="nav-item">{{
          link.name
        }}</router-link>
      </div>
    </div>
    <div class="messager-nav">
      <div class="logomessage">
        <img src="../assets/image/f.png" alt="logo" class="logo-ms" />
      </div>
      <div class="logomessage">
        <img src="../assets/image/twitter.png" alt="logo" class="logo-ms" />
      </div>
      <div class="logomessage">
        <img src="../assets/image/linked_in.png" alt="logo" class="logo-ms" />
      </div>
      <div class="logomessage">
        <img src="../assets/image/bg.png" alt="logo" class="logo-ms" />
      </div>
      <div class="logomessage">
        <img src="../assets/image/instagram.png" alt="logo" class="logo-ms" />
      </div>
    </div>
  </header>
  <div class="botton-header">
    <p>
      Congratulations to our dear friends and colleagues... Receiving the
      highest award and gold medal from the World Federation of Inventors in
    </p>
  </div>
</template>

<script>
const navLink = [
  { path: "/home", name: "HOME" },
  { path: "/prodacts", name: "PRODUCTS" },
  { path: "/about", name: "ABOUT US" },
  { path: "/investor", name: "INVESTOR" },
  { path: "/download", name: "DOWNLOAD" },
  { path: "/link", name: "LINK" },
  { path: "/rod", name: "R&D" },
  { path: "/exhibition", name: "EXHIBITION" },
  { path: "/contact", name: "CONTACT US" },
];

export default {
  data() {
    return {
      linkNav: navLink,
      closes: false,
    };
  },
  methods: {
    close() {
      this.closes = !this.closes;
    },
    opeenNav() {
      this.closes = !this.closes;
    },
  },
};
</script>

<style scoped>
@import '../assets/styles/header.css';
</style>