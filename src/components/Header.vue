<template>
  <header>
    <h1>Daniel Machado</h1>
  </header>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style scoped>
header {
  background-image: url("https://images.unsplash.com/photo-1528722828814-77b9b83aafb2?ixlib=rb-1.2.1&w=1000&q=80");

  height: 400px;

  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  display: flex;

  align-items: center;
  justify-content: center;
}

h1 {
  color: white;
}
</style>