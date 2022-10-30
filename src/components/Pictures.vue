<template>
  <section>
    <div class="all-box">
      <div class="container">
        <div class="btn-back"><img src="../assets/image/vector4.png" alt=""></div>
        <div class="main-box">
          <h2>Pictures</h2>
          <div class="box-slider">
                <div class="photo-sloider">
                    <img src="../assets/image/Rectangle 1161.png" alt="">
                    <div class="hover-photo"><p class="name-view">View</p></div>
                    <p>About picture</p>
                </div>
                <div class="photo-sloider1">
                    <img src="../assets/image/Rectangle 1161.png" alt="" class="img-main">
                    <div class="hover-photo"><p class="name-view">View</p></div>
                    <p>About picture About picture About picture About picture</p>
                </div>
                <div class="photo-sloider">
                    <img src="../assets/image/Rectangle1255548.png" alt="">
                    <div class="hover-photo"><p class="name-view">View</p></div>
                    <p>About picture About picture About </p>
                </div>
          </div>
          <div class="pointer">
            <div class="point"></div>
            <div class="point"></div>
            <div class="point"></div>
            <div class="point1"></div>
            <div class="point"></div>
            <div class="point"></div>
            <div class="point"></div>
          </div>
        </div>
        <div class="btn-next"><img src="../assets/image/vector5.png" alt=""></div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.all-box {
  width: 100%;
  height: 508px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #ffffff;
}
.container {
    width: 75%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
.main-box{
    width: 75%;
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #325E6A;
}
.name-view{
    margin-top: 10px;
}
.btn-back {
    cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 35px;
  height: 38px;
  background-image: url("../assets/image/Polygon2.png");
}
.btn-next{
    cursor: pointer;
    display: flex;
  justify-content: center;
  align-items: center;
  width: 35px;
  height: 38px;
  background-image: url("../assets/image/Polygon2.png");
}
.photo-sloider{
  position: relative;
    width: 267px;
    height: 250px;
    margin: 0 15px;
    
}

.photo-sloider1{
  position: relative;
    width: 267px;
    height: 250px;
    margin: 0 15px;

}
.box-slider{
    display: flex;
    flex-direction: row;
    justify-content: space-around;
}
.pointer{
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.point{
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: rgb(225, 222, 222);
  margin: 0 7px;
  margin-top: 50px;
}
.point:hover{
  background: #008BDE;
}
.point1{
    width: 8px;
  height: 8px;
  border-radius: 50%;
  background: #008BDE;
  margin: 0 7px;
  margin-top: 50px;
}
.hover-photo{
    cursor: pointer;
    position: absolute;
    left: 100px;
    top: 100px;
    width: 99px;
    border-radius: 10px;
    height: 48px;
    background: rgba(255, 255, 255, 0.9);
    color: #325E6A;
    font-size: 18px;
    font-weight: 500;
    text-align: center;
    display: none;
}
.img-main:hover{
    opacity: calc(0.7);
}
.photo-sloider1:hover .hover-photo{
    display: inline;
}
.photo-sloider:hover .hover-photo{
    display: inline;
}
</style>