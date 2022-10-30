<template>
  <main>
    <div class="main-img">
      <div class="model">
        <div class="img-back"><img src="../assets/image/Vector2.png" alt="" /></div>
        <div class="all-div">
          <div class="banner-head"><h2>SLEER</h2></div>
          <div class="main-main">
            <p>
              What could be better than combining the best coffees in the
              fastest time possible! We are there easily whenever you want.Get
              hot drinks like coffee and cappuccino as soon as possible.
            </p>
          </div>
          <div class="button-Project">See Project</div>
        </div>
        <div  class="img-next"><img src="../assets/image/Vector3.png" alt="" /></div>
      </div>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<style scoped>
.main-img {
  display: flex;
  justify-content: center;
  flex-direction: row;
  align-items: center;
  width: 100%;
  height: 896px;
  background-image: url("../assets/image/men.png");
}
.model {
  width: 70%;
  display: flex;
  justify-content: center;
  flex-direction: row;
  align-items: center;
}
.banner-head {
  font-weight: 900;
  font-size: 60px;
  color: white;
  display: flex;
  justify-content: center;
}
.all-div{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

}
.main-main{
    width: 75%;
    margin-top: -50px;
    color: white;
    font-size: 20px;
    padding: 0 50px;
}
.img-back{
  text-align: center;
  align-items: center;
}
.img-back:hover{
    opacity: calc(0.5);
}
.button-Project{
    width: 170px;
    height: 51px;
    background: #008BDE;
    border-radius: 24px;
    color: #EDEDED;
    font-size: 24px;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
}

.img-next{
    text-align: center;
  align-items: center;
}
.img-next:hover{
    opacity: calc(0.5);
}
</style>