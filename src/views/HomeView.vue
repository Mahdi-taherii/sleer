<script>
import Header from "../components/Header.vue";
import MainPhoto from "../components/MainPhoto.vue";
import Rectangle from "../components/Rectangle.vue";
import Pictures from "../components/Pictures.vue";
import Tables from "../components/Tables.vue";
import Videos from "../components/Videos.vue";
import Suppliers from '../components/Suppliers.vue'
export default {
  components: { Header, MainPhoto, Rectangle, Pictures, Tables, Videos ,Suppliers  },

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
  <Videos/>
  <Suppliers/>
</template>
