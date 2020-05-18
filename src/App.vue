<template>
  <div id="app">
    <Header />
    <Menu />
    <Body />
  </div>
</template>

<script>
import { Header, Menu, Body } from "./components/index.js";

export default {
  name: "App",
  components: { Header, Menu, Body }
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
