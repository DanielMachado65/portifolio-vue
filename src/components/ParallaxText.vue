<template>
  <div class="layer parallax-text">
    <a href="#" class="btn">Compartilhe!</a>

    <div class="container-center">
      <h1>Daniel</h1>
      <h2>Um pouco da história</h2>
    </div>

    <div class="social-container">
      <a href="https://www.instagram.com/morenauum/" target="_blank">
        <i class="icon ion-logo-facebook"></i>
      </a>
      <a href="https://github.com/DanielMachado65" target="_blank">
        <i class="icon ion-logo-github"></i>
      </a>
      <a href="https://www.instagram.com/morenauum/" target="_blank">
        <i class="icon ion-logo-instagram"></i>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "ParallaxText"
};
</script>

<style>
.parallax-text {
  z-index: 6;
  display: flex;
  justify-content: center;
  align-items: center;
}

.parallax-text .btn{
  position: absolute;
  left: 2rem;
  top: 2rem;
}

.container-center h2{
  background: coral;
}

.social-container {
  position: absolute;
  right: 2.5rem;
  bottom: 2.5rem;
}

.social-container i {
  font-size: 2rem;
  margin-right: 0.8rem;
}

</style>