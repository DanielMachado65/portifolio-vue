<template>
  <div class="parallax-group hero-container">
    <div class="layer sky"></div>
    <div class="layer main"></div>
    <div class="layer house1"></div>
    <div class="layer house2"></div>
    <div class="layer lion"></div>
    <parallax-text />
  </div>
</template>

<script>
import ParallaxText from "./ParallaxText.vue";

export default {
  name: "Parallax",
  components: { ParallaxText }
};
</script>

<style>
.layer {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
}

.sky {
  background: url("../assets/sky.png") no-repeat center;
  background-size: cover;
  transform: translateZ(-600px) scale(3);
  z-index: 1;
}

.main {
  background: url("../assets/main.png") no-repeat center;
  background-size: cover;
  transform: translateZ(-400px) scale(2.33333333);
  z-index: 2;
}

.house1 {
  background: url("../assets/house1.png") no-repeat center;
  background-size: cover;
  transform: translateZ(-250px) scale(1.833333333);
  z-index: 3;
}

.house2 {
  background: url("../assets/house2.png") no-repeat center;
  background-size: cover;
  transform: translateZ(-125px) scale(1.4167);
  z-index: 4;
}

.lion {
  background: url("../assets/lion.png") no-repeat center;
  background-size: cover;
  transform: translateZ(0) scale(1);
  z-index: 5;
}
</style>