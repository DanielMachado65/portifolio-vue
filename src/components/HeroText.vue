<template>
  <div class="layer hero-text">
    <h2>Level Up Inc.</h2>

    <div class="container-center">
      <h1>Daniel</h1>
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
  name: "HeroText"
};
</script>

<style>
.hero-text {
  z-index: 6;

  display: flex;
  justify-content: center;
  align-items: center;
}

.container-center {
  background: coral;
}

.hero-text h2 {
  font-size: 1.25rem;
  position: absolute;
  left: 2.5rem;
  top: 2.5rem;
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

@media (min-width: 760px) {
  .hero-text ul {
    visibility: visible;
  }
}
</style>