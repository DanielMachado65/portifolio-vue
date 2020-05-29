<template>
  <div class="layer hero-text">
    <h2>Level Up Inc.</h2>
    <ul>
      <li>
        <a href="#">Passions</a>
      </li>
      <li>
        <a href="#">Goals</a>
      </li>
      <li>
        <a href="#" class="btn">Get Started Now</a>
      </li>
    </ul>
    <div class="year-container">
      <h1>Daniel</h1>
    </div>
    <div class="social-container">
      <a href="https://github.com/KiaanCastillo" target="_blank">
        <i class="icon ion-logo-github"></i>
      </a>
      <a href="https://www.instagram.com/craftedbykiaan/" target="_blank">
        <i class="icon ion-logo-instagram"></i>
      </a>
      <a href="https://dribbble.com/kiaancastillo" target="_blank">
        <i class="icon ion-logo-dribbble"></i>
      </a>
      <a href="https://www.youtube.com/c/KiaanCastillo" target="_blank">
        <i class="icon ion-logo-youtube"></i>
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
  background-size: cover;
  transform: translateZ(0) scale(1);
  z-index: 7;
}

.hero-text h2 {
  font-size: 1.25rem;
  position: absolute;
  left: 2.5rem;
  top: 2.5rem;
}

.hero-text ul {
  font-size: 0.75rem;
  position: absolute;
  right: 2.5rem;
  top: 2.5rem;
}

.hero-text ul li {
  margin-left: 2.5rem;
  list-style-type: none;
  float: left;
  visibility: hidden;
}

.hero-text ul li:nth-of-type(3) {
  visibility: visible;
}

.year-container {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  height: 10rem;
  width: 15rem;
}

.year-container h1 {
  font-weight: bold;
  position: absolute;
  font-size: 4rem;
}

.social-container {
  position: absolute;
  left: 2.5rem;
  bottom: 2.5rem;
}

.social-container i {
  font-size: 1.25rem;
  margin-right: 0.25rem;
}

@media (min-width: 760px) {
  .hero-text ul {
    visibility: visible;
  }
}
</style>