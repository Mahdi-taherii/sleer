<script>
import Header from "../components/Header.vue";
import MainPhoto from "../components/MainPhoto.vue";
import Rectangle from "../components/Rectangle.vue";
import Pictures from "../components/Pictures.vue";
import Tables from "../components/Tables.vue";
import Videos from "../components/Videos.vue";
import Suppliers from "../components/Suppliers.vue";
import Process from "../components/Process.vue";

const user = [
  {
    id: 1,
    url: "../assets/image/img/Rectangle 1200.png",
    title: "Donald Norman",
    disripton: "Scrum Master",
  },
  {
    id: 2,
    url: "../assets/image/img/Rectangle 1201.png",
    title: "Mia sozie",
    disripton: "Designer",
  },
  {
    id: 3,
    url: "../assets/image/img/Rectangle 1202.png",
    title: "Tommy Slazer",
    disripton: "Front end developer",
  },
  {
    id: 4,
    url: "../assets/image/img/Rectangle 1207.png",
    title: "Sura Smilez",
    disripton: "owner",
  },
  {
    id: 5,
    url: "../assets/image/img/Rectangle 1209.png",
    title: "Lucy spark",
    disripton: "Researcher",
  },
  {
    id: 6,
    url: "../assets/image/img/Rectangle 1208.png",
    title: "Antonio Guadrivol",
    disripton: "Information Arcitecture",
  },
  {
    id: 7,
    url: "../assets/image/img/Rectangle 1210.png",
    title: "Santos Marino",
    disripton: "Back end developer",
  },
];
export default {
  components: {
    Header,
    MainPhoto,
    Rectangle,
    Pictures,
    Tables,
    Videos,
    Suppliers,
    Process,
  },
  data() {
    return {
      users: user,
    };
  },
  methods: {
    text() {
      console.log(this.$attrs);
    },
  },
};
</script>

<template>
  <Header />
  <MainPhoto />
  <Rectangle />
  <Pictures />
  <Tables />
  <Videos />
  <Suppliers />
  <Process />
  <div class="colleagues">
    <div class="container1">
      <div class="text-title"><h2>Our colleagues</h2></div>
      <div class="profile">
        <div class="add-card">
          <img src="../assets/image/Group 1914.png" alt="" />
        </div>
        <div class="img-profile" v-for="user in users" :key="user.id">
          <img
            src="../assets/image/img/Rectangle 1202.png"
            alt=""
            class="image-hover"
          />
          <div class="box-title">
            <h2 class="title-photo">{{ user.title }}</h2>
            <p class="discription">{{ user.disripton }}</p>
          </div>
          <div class="box-logo1">
            <img src="../assets/image/linked_in.png" alt="" />
            <div class="slider-hover">{{ user.title }}</div>
          </div>
          <div class="box-logo2">
            <img src="../assets/image/twitter.png" alt="" />
            <div class="slider-hover">{{ user.title }}</div>
          </div>
          <div class="box-logo3">
            <img src="../assets/image/f.png" alt="" />
            <div class="slider-hover">{{ user.title }}</div>
          </div>
          <div class="box-logo4">
            <img src="../assets/image/logo/vector10.png" alt="" />
            <div class="slider-hover">{{ user.title }}</div>
          </div>
          <div class="box-logo5">
            <img src="../assets/image/instagram.png" alt="" />
            <div class="slider-hover">{{ user.title }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="Contact">
    <div class="text-Contact"><h2>Contact us</h2></div>
    <div class="colaps">
      <div class="form-Contact">
        <form>
          <h3>
            You can <span class="text-blue">contact me</span> by filling out
            this form
          </h3>
          <div class="input-name">
            <img
              src="../assets/image/img/vector.png"
              alt=""
              width="14"
              height="9"
              class="logo-user1"
            />
            <img
              src="../assets/image/img/vector1.png"
              alt=""
              width="8"
              height="8"
              class="logo-user2"
            />
            <input type="text" placeholder="Your name" class="input-1" />
          </div>
          <div class="input-email">
            <img
              src="../assets/image/img/vector3.png"
              alt=""
              width="17"
              height="17"
              class="logo-user3"
            />
            <img
              src="../assets/image/img/vector6.png"
              alt=""
              width="7"
              height="7"
              class="logo-user4"
            />
            <input type="text" placeholder="Your Email" class="input-2" />
          </div>
          <div class="text-message">
            <img
              src="../assets/image/img/vector7.png"
              alt=""
              width="17"
              height="17"
              class="logo-user5"
            />
            <img
              src="../assets/image/img/vector8.png"
              alt=""
              width="7"
              height="7"
              class="logo-user6"
            />
            <textarea placeholder="Messeage" class="input-3"></textarea>
          </div>
          <button class="submit">Submit</button>
        </form>
      </div>
      <div class="about-contact">
        <h3>Know a little about me</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas
          purus viverra accumsan in nisl nisi. Arcu cursus vitae congue mauris
          rhoncus aenean vel elit scelerisque. In egestas erat imperdiet sed
          euismod nisi porta lorem mollis. Morbi tristique senectus et netus.
          Mattis pellentesque id nibh tortor id aliquet lectus proin. Sapien
          faucibus et molestie ac feugiat sed lectus vestibulum. Ullamcorper
          velit sed ullamcorper morbi tincidunt ornare massa eget. Dictum
        </p>
      </div>
    </div>
  </div>
  <footer class="footer">
    <div class="all-footer">
      <div class="about-footer">
        <div class="logo-footer">
          <img src="../assets/image/image1.png" alt="" />
        </div>
        <h3>
          Sleer Investor Relations website at
          http://www.somitra.com/index.php/investment and our corporate blog at
          sleer.nl, as well as Sleer social media accounts, contain a
          significant amount of information about R&D, including financial and
          other information for investors.
        </h3>
      </div>
      <div class="title-footer">
        <h3>QUICK ACCESS</h3>
        <h4>Home</h4>
        <h4>About us</h4>
        <h4>Investor</h4>
        <h4>Links</h4>
        <h4>Blog</h4>
        <h4>Download</h4>
        <h4>Contact</h4>
      </div>
      <div class="map-footer"></div>
      <div class="programing">
        <div class="program-logo">
          <img src="../assets/image/logo/f.png" alt="" />
        </div>
        <div class="program-logo">
          <img src="../assets/image/logo/twitter.png" alt="" />
        </div>
        <div class="program-logo">
          <img src="../assets/image/logo/linked_in.png" alt="" />
        </div>
        <div class="program-logo">
          <img src="../assets/image/logo/bg.png" alt="" />
        </div>
        <div class="program-logo">
          <img src="../assets/image/logo/instagram.png" alt="" />
        </div>
      </div>
    </div>
  </footer>
  <div class="button-footer"></div>
</template>

<style scoped>
@import "../assets/styles/homeview.css";
</style>
