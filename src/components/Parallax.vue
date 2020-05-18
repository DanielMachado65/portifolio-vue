<template>
  <v-container>
    <header>
      <div class="parallax-layer layer-0">
        <img
          src="https://github.com/samdbeckham/blog/blob/master/dev/_assets/images/articles/firewatch/layer_0.png?raw=true"
        />
      </div>
      <div class="parallax-layer layer-1">
        <img
          src="https://github.com/samdbeckham/blog/blob/master/dev/_assets/images/articles/firewatch/layer_1.png?raw=true"
        />
      </div>
      <div class="parallax-layer layer-2">
        <img
          src="https://github.com/samdbeckham/blog/blob/master/dev/_assets/images/articles/firewatch/layer_2.png?raw=true"
        />
      </div>
      <div class="parallax-layer layer-3">
        <img
          src="https://github.com/samdbeckham/blog/blob/master/dev/_assets/images/articles/firewatch/layer_3.png?raw=true"
        />
      </div>
      <div class="parallax-layer layer-4">
        <img
          src="https://github.com/samdbeckham/blog/blob/master/dev/_assets/images/articles/firewatch/layer_4.png?raw=true"
        />
      </div>
      <div class="parallax-layer layer-5">
        <img
          src="https://github.com/samdbeckham/blog/blob/master/dev/_assets/images/articles/firewatch/layer_5.png?raw=true"
        />
      </div>
      <div class="parallax-layer layer-6">
        <img
          src="https://github.com/samdbeckham/blog/blob/master/dev/_assets/images/articles/firewatch/layer_6.png?raw=true"
        />
      </div>
      <main>
        <slot></slot>
      </main>
    </header>
  </v-container>
</template>

<script>
export default {
  name: "Parallax"
};
</script>

<style scoped>
header {
  perspective: 100px;
  height: 100vh;
  overflow-x: hidden;
  overflow-y: auto;
  position: absolute;
  top: 0;
  left: 50%;
  right: 0;
  bottom: 0;
  margin-left: -1500px;
}
main {
  background: #2d112b;
  display: block;
  position: absolute;
  top: 100%;
  left: 0;
  right: 0;
  height: 2000px;
  z-index: 2;
}
.parallax-layer {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
}
.parallax-layer img {
  display: block;
  position: absolute;
  bottom: 0;
}
.layer-0 {
  transform: translateZ(-300px) scale(4);
}
.layer-1 {
  transform: translateZ(-250px) scale(3.5);
}
.layer-2 {
  transform: translateZ(-200px) scale(3);
}
.layer-3 {
  transform: translateZ(-150px) scale(2.5);
}
.layer-4 {
  transform: translateZ(-100px) scale(2);
}
.layer-5 {
  transform: translateZ(-50px) scale(1.5);
}
.layer-6 {
  transform: translateZ(0px) scale(1);
}
</style>