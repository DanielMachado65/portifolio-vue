<template>
  <div id="app">
    <Parallax>

    </Parallax>
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
body {
  margin: 0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
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
