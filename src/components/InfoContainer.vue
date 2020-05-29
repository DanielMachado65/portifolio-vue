<template>
  <div class="parallax-group info-container">
    <img src="../assets/main.png" alt="Lively and colourful concert" />
    <div class="text-container">
      <h2>This is your year.</h2>
      <p>What would life be if we had no courage to attempt anything?</p>
      <p>- Vincent Van Gogh</p>
      <a href="#" class="btn">Get Started Now</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "InfoContainer"
};
</script>

<style>
.info-container {
  background: #000;
  transform: translateZ(0) scale(1);
  z-index: 8;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.info-container img {
  width: 75%;
  margin-bottom: 2.5rem;
  filter: saturate(0.65);
}

.info-container h2,
.info-container p {
  margin-bottom: 1rem;
}

.text-container p:nth-of-type(1) {
  font-weight: 400;
  font-size: 0.75rem;
  margin: 1rem 2.5rem;
}

.text-container p:nth-of-type(2) {
  font-size: 0.6rem;
  margin-bottom: 3rem;
}

@media (min-width: 760px) {
  .info-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-column-gap: 3rem;
    align-items: center;
    text-align: left;
  }

  .info-container img {
    justify-self: end;
    width: 75%;
  }
}
</style>