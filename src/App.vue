<template>
  <div id="app">
    <Parallax />
    <info-container />
  </div>
</template>

<script>
import Parallax from "./components/Parallax.vue";
import InfoContainer from "./components/InfoContainer.vue";

export default {
  name: "App",
  components: { Parallax, InfoContainer }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap");

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html,
body {
  width: 100%;
  height: 100%;
  color: #fff;
  background-color: #000;
  font-family: Montserrat, Arial, Helvetica, sans-serif;
  font-weight: 700;
}

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

.btn:hover {
  color: #000;
  background: #fff;
}

#app {
  height: 100vh;
  overflow-x: hidden;
  overflow-y: auto;
  perspective: 300px;
}

.parallax-group {
  position: relative;
  height: 100vh;
  width: 100vw;
  transform-style: preserve-3d;
}
</style>
