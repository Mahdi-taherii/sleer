<script>
import Header from "../components/Header.vue";
import MainPhoto from "../components/MainPhoto.vue";
import Rectangle from "../components/Rectangle.vue";
import Pictures from "../components/Pictures.vue";
import Tables from "../components/Tables.vue";
import Videos from "../components/Videos.vue";
import Suppliers from '../components/Suppliers.vue'
import Process from '../components/Process.vue'
export default {
  components: { Header, MainPhoto, Rectangle, Pictures, Tables, Videos ,Suppliers , Process  },

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
  <Process/>
  <div  class="colleagues">
    
  </div>
</template>

<style scoped>

</style>
