<template>
  <HeroBanner />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HeroBanner from "./components/HeroBanner.vue";

export default defineComponent({
  name: "App",
  components: {
    HeroBanner,
  },
});
</script>

<style lang="scss">
@import "./styles/styles.scss";
body {
  background: $base-color;
  background-image: radial-gradient(rgba(256,256,256,0.4) 1px, transparent 0);
  background-size: 40px 40px;
  background-position: -19px -19px;

  overflow-x: hidden;
}
h1 {
  font-size: $header-1;
  margin: 0;
  font-weight: 400;
}
h2 {
  font-size: $header-2;
  font-weight: 400;
  margin: 0;
}

h3 {
  font-size: $header-3;
  font-weight: 400;
  margin: 0;
}
h4 {
  font-size: $header-4;
  font-weight: 400;
  margin: 0;
}
p {
  font-size: $paragraph;
  font-weight: 400;
  margin: 0;
}

#app {
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: $foreground-text;
  position: relative;
  max-width: 2560px;
  margin: 0 auto;
  margin-top: 80px;
  padding: 30px;
}
</style>
