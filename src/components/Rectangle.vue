<template>
  <div class="main-rec">
    <div class="main-box-blue">
      <div class="div-white">
        <div class="btn-back"><img src="../assets/image/vector4.png" alt=""></div>
        <div class="main-text">
          <h2 class="heade-text">ADVANTAGES OF ECONOMICAL COMBINED METER</h2>
          <p>
            In 2017, the Board of Directors decided to work on this project at
            the national level and asked the research team to work on producing
            smart electric meters which would never have a similar prototype.
            Our company had the experience of designing smart home and
            industrial electronic circuit boards which perform like a smart
            meter. Subsequently, following these experiences helped us to
            succeed in building a cumulative smart meter after nearly two years.
            We met our goals with this one.
          </p>
          <div class="pointer">
            <div class="point"></div>
            <div class="point"></div>
            <div class="point1"></div>
            <div class="point"></div>
            <div class="point"></div>
          </div>
        </div>
        <div class="btn-next"><img src="../assets/image/vector5.png" alt=""></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.main-rec {
  width: 100%;
  height: 642px;
  background: #F4F8FD;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.main-box-blue {
  width: 1140px;
  height: 384px;
  background: #008bde;
  border-radius: 10px;
  transform: rotate(-5deg);
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.05);
}
.div-white {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  background: #ffffff;
  width: 1140px;
  height: 384px;
  transform: rotate(5deg);
  border-radius: 10px;
}
.heade-text {
  font-size: 24px;
  color: #325e6a;
}
p {
  color: #325e6a;
  font-size: 16px;
}
.main-text{
  width: 75%;
  text-align: center;
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
.btn-next {
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 35px;
  height: 38px;
  background-image: url("../assets/image/Polygon2.png");
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
.point1{
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: #FF9C00;
  margin: 0 7px;
  margin-top: 50px;
}
</style>