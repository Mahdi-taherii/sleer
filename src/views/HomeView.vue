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
    url: "../assets/image/img/Rectangle 1200.png",
    title: "Donald Norman",
    disripton: "Scrum Master",
  },
  {
    url: "../assets/image/img/Rectangle 1201.png",
    title: "Mia sozie",
    disripton: "Designer",
  },
  {
    url: "../assets/image/img/Rectangle 1202.png",
    title: "Tommy Slazer",
    disripton: "Front end developer",
  },
  {
    url: "../assets/image/img/Rectangle 1207.png",
    title: "Sura Smilez",
    disripton: "owner",
  },
  {
    url: "../assets/image/img/Rectangle 1209.png",
    title: "Lucy spark",
    disripton: "Researcher",
  },
  {
    url: "../assets/image/img/Rectangle 1208.png",
    title: "Antonio Guadrivol",
    disripton: "Information Arcitecture",
  },
  {
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
        <div class="img-profile" v-for="user in users" :key="user">
          <img src="../assets/image/img/Rectangle 1201.png" alt="" />
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
            <img src="../assets/image/img/vector.png" alt="" />
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
</template>

<style scoped>
.colleagues {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  height: 900px;
  background: #f4f8fd;
}
.container1 {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  flex-direction: column;
  align-items: center;
  width: 90%;
}
.text-title {
  font-weight: 700;
  font-size: 25px;
  color: #325e6a;
}
.profile {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}
.add-card {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 279px;
  height: 422px;
  background: #325e6a;
  box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.05);
  border-radius: 10px;
  cursor: pointer;
}
.img-profile {
  position: relative;
  width: 279px;
  height: 422px;
}
.box-logo1 {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  left: 10px;
  top: 10px;
  width: 32px;
  height: 32px;
  background: rgba(255, 255, 255, 0.5);
  border-radius: 29px;
  display: none;
}
.profile:hover .box-logo1 {
  display: inline-flex;
}
.profile:hover .box-logo2 {
  display: inline-flex;
}
.profile:hover .box-logo3 {
  display: inline-flex;
}
.profile:hover .box-logo4 {
  display: inline-flex;
}
.profile:hover .box-logo5 {
  display: inline-flex;
}
.box-logo1:hover {
  background: #ff8800;
}
.box-logo2:hover {
  background: #ff9c00;
}
.box-logo3:hover {
  background: #ff9c00;
}
.box-logo4:hover {
  background: #ff9c00;
}
.box-logo5:hover {
  background: #ff9c00;
}
.box-logo2 {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  left: 10px;
  top: 50px;
  width: 32px;
  height: 32px;
  background: rgba(255, 255, 255, 0.5);
  border-radius: 29px;
  display: none;
}
.box-logo3 {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  left: 10px;
  top: 90px;
  width: 32px;
  height: 32px;
  background: rgba(255, 255, 255, 0.5);
  border-radius: 29px;
  display: none;
}
.box-logo4 {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  left: 10px;
  top: 130px;
  width: 32px;
  height: 32px;
  background: rgba(255, 255, 255, 0.5);
  border-radius: 29px;
  display: none;
}
.box-logo5 {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  left: 10px;
  top: 170px;
  width: 32px;
  height: 32px;
  background: rgba(255, 255, 255, 0.5);
  border-radius: 29px;
  display: none;
}
.slider-hover {
  position: absolute;
  border-radius: 16px;
  left: 0px;
  width: 130px;
  height: 32px;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0 10px;
  color: white;
  font-size: 12px;
  background: rgba(255, 255, 255, 0.4);
  display: none;
}
.box-logo1:hover .slider-hover {
  display: inline-flex;
}
.box-logo2:hover .slider-hover {
  display: inline-flex;
}
.box-logo3:hover .slider-hover {
  display: inline-flex;
}
.box-logo4:hover .slider-hover {
  display: inline-flex;
}
.box-logo5:hover .slider-hover {
  display: inline-flex;
}
.box-title {
  position: absolute;
  left: 15px;
  top: 320px;
  color: white;
}
</style>
