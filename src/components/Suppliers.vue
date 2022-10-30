<template>
  <div class="container">
    <div class="main-box">
      <div class="text-title"><h2>Our Suppliers</h2></div>
      <div>
        <img src="../assets/image/Rectangle 1194.png" alt=""  class="img-brand"/>
        <img src="../assets/image/Rectangle 1169.png" alt=""  class="img-brand"/>
        <img src="../assets/image/Rectangle 1170.png" alt=""  class="img-brand"/>
        <img src="../assets/image/Rectangle 1171.png" alt=""  class="img-brand"/>
        <img src="../assets/image/Rectangle 1172.png" alt=""  class="img-brand"/>
        <img src="../assets/image/Rectangle 1194.png" alt=""  class="img-brand"/>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  background: #f5f5f5;
  width: 100%;
  height: 350px;
}
.main-box {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}
.text-title {
  font-weight: 700;
  font-size: 28px;
  color: #325E6A;
}
.img-brand:hover{
  opacity: 0.8;
  width: 202px;
}
</style>