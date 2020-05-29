<template>
  <div class="parallax-group info-container">
    <div class="text-container">
      <iframe src="https://open.spotify.com/embed/track/0PXukVbYpvz40KcEFKnIw7" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
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
</style>