<template>
  <div class="logoGosp">
    <img class="logoGosp_carrot" src="@/static/images/carrot.png" alt="localgosp">
    <img class="logoGosp_ribbon" src="@/static/images/ribbon.png" alt="localgosp">
    <span class="logoGosp_title">LocalGosp</span>
  </div>
</template>

<style lang="scss">
img {
  max-width: 100%;
}
.logoGosp {
  position: relative;
  float: left;
  width: 150px;
  height: 15vh;
  border-radius: 50%;
  background-color: #cbf442;

  &_carrot {
    position: absolute;
    top:0;
    left: 0;
  }

  &_ribbon {
    position: absolute;
    z-index: 1;
    top: 75%;
    left: 0px;
  }

  &_title {
    position: absolute;
    top: 80%;
    left: 20%;
    color: #f44141;
    text-shadow: 1px 1px 0px black;
    font-size: 20px;
    z-index: 2;
  }
}
</style>
