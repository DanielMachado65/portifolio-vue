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
:root {
  --webkit-font-smoothing: antialiased;
  --moz-ozx-font-smoothing: grayscale;
}

body {
  color: #fff;
  background: rgb(65, 38, 19);
  background: linear-gradient(
    0deg,
    rgba(65, 38, 19, 0.9136029411764706) 0%,
    rgba(92, 147, 178, 0.8939950980392157) 96%
  );
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
  overflow: hidden;
  position: relative;
  height: 100vh;
  width: 100vw;
  transform-style: preserve-3d;
}

::-webkit-scrollbar {
  width: 0.25rem;
}

::-webkit-scrollbar-track {
  background: #1e1e24;
}

::-webkit-scrollbar-thumb {
  background: coral;
}
</style>
