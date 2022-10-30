<template>
  <header>
    <div class="logo-nav">
      <img src="../assets/image/image1.png" alt="logo" class="logo-img" />
    </div>
    <div class="nav-link">
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
    };
  },
};
</script>

<style scoped>
header {
  background: #008bde;
  height: 64px;
  display: flex;
  align-items: center;
}
.logo-nav {
  font-size: 14px;
}
.nav-item {
  text-decoration: none;
  color: white;
  letter-spacing: 1px;
}
.nav-item:hover {
  color: black;
}
.div-item {
  display: inline;
  padding: 0 10px;
}
.logo-img {
  padding: 0 15px;
  width: 80px;
}
.messager-nav {
  width: 15%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin-left: 10%;
  margin-right: 2%;
}
.logo-ms {
  padding: 10px;
}
.logomessage {
  margin: 0 7px;
  border-radius: 10px;
  background: #325e6a;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 32px;
  width: 32px;
}
.botton-header {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 40px;
  background: #325e6a;
}
.botton-header p {
  font-size: 16px;
  margin: 0;
  color: white;
}
</style>