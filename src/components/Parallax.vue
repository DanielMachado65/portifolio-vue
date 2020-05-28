<template>
  <div class="parallax-group hero-container">
    <div class="layer sky"></div>
    <div class="layer bushes"></div>
    <div class="layer water"></div>
    <div class="layer people1"></div>
    <div class="layer people2"></div>
    <div class="layer people3"></div>
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
        <h1>2</h1>
        <h1>0</h1>
        <h1>1</h1>
        <h1>9</h1>
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
  </div>
</template>

<script>
export default {
  name: "Parallax"
};
</script>

<style>


a {
  text-decoration: none;
  color: #fff;
}

.btn {
  border: 1.5px solid #fff;
  border-radius: 0.75rem;
  padding: 0.75rem 1.25rem;
  transition: all 0.3s ease-in-out;
}

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

.bushes {
  background: url("../assets/bushes.png") no-repeat center;
  background-size: cover;
  transform: translateZ(-525px) scale(2.75);
  z-index: 2;
}

.water {
  background: url("../assets/water.png") no-repeat center;
  background-size: cover;
  transform: translateZ(-400px) scale(2.33333333);
  z-index: 3;
}

.people1 {
  background: url("../assets/people1.png") no-repeat center;
  background-size: cover;
  transform: translateZ(-250px) scale(1.833333333);
  z-index: 4;
}

.people2 {
  background: url("../assets/people2.png") no-repeat center;
  background-size: cover;
  transform: translateZ(-125px) scale(1.4167);
  z-index: 5;
}

.people3 {
  background: url("../assets/people3.png") no-repeat center;
  background-size: cover;
  transform: translateZ(0) scale(1);
  z-index: 6;
}

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
  width: 17rem;
  height: 25rem;
}

.year-container h1 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  position: absolute;
  font-size: 9.5rem;
}

.year-container h1:nth-of-type(1) {
  top: 10%;
}

.year-container h1:nth-of-type(2) {
  left: 30%;
  bottom: 0;
}

.year-container h1:nth-of-type(3) {
  top: 0;
  right: 30%;
}

.year-container h1:nth-of-type(4) {
  right: 0;
  bottom: 20%;
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
  .hero-text ul li {
    visibility: visible;
  }
  
  .text-container p:nth-of-type(1) {
    font-size: 1rem;
    width: 75%;
    margin: 1rem 0;
  }

  .text-container p:nth-of-type(1) {
    font-size: 0.86rem;
  }
}


</style>