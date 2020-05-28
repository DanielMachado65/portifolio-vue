<template>
  <div id="app">
    <Parallax />
    <v-container class="parallax-group">
      <v-row>aksjdsad</v-row>
    </v-container>
  </div>
</template>

<script>
import Parallax from "./components/Parallax.vue";

export default {
  name: "App",
  components: { Parallax }
};
</script>

<style>
:root {
  --webkit-font-smoothing: antialiased;
  --moz-ozx-font-smoothing: grayscale;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html,
body {
  width: 100%;
  height: 100%;
  color: #ffffff;
  background-color: #000;
  font-family: Arial, Helvetica, sans-serif;
}

#app{
  height: 100vh;
  overflow-x: hidden;
  overflow-y: auto;
  perspective: 300px;
}

.parallax-group{
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
  background: #000328;
}
</style>
