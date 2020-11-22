<template>
  <HeroBanner />
  <TechStack />
  <Experience />
  <Contact />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import TechStack from "./sections/TechStack-section.vue";
import HeroBanner from "./sections/HeroBanner-section.vue";
import Experience from "./sections/Experience-section.vue";
import Contact from "./sections/Contact-section.vue";

export default defineComponent({
  name: "App",
  components: {
    HeroBanner,
    TechStack,
    Experience,
    Contact,
  },
});
</script>

<style lang="scss">
@import "./styles/styles.scss";
body {
  background: $base-color;
  background-image: radial-gradient(
    rgba(256, 256, 256, 0.4) 0.7px,
    transparent 0
  );
  background-size: 40px 40px;
  background-position: -19px -19px;

  overflow-x: hidden;
}
h1 {
  font-size: $header-big-1;
  margin: 0;
  font-weight: 400;
}

h2 {
  font-size: $header-big-2;
  font-weight: 400;
  margin: 0;
}

h3 {
  font-size: $header-big-3;
  font-weight: 400;
  margin: 0;
}

@media only screen and (max-width: 1575px) {
  h1 {
    font-size: $header-mid-1;
  }
  h2 {
    font-size: $header-mid-2;
  }
  h3 {
    font-size: $header-mid-3;
  }
}

@media only screen and (max-width: 768px) {
  h1 {
    font-size: $header-small-1;
  }
  h2 {
    font-size: $header-small-2;
  }
  h3 {
    font-size: $header-small-3;
  }
}

h4 {
  font-size: $header-4;
  font-weight: 400;
  margin: 0;
}

h5 {
  font-size: $header-5;
  font-weight: 400;
  margin: 0;
}

h6 {
  font-size: $header-6;
  font-weight: 200;
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
  max-width: 1575px;
  margin: 0 auto;
  padding: 30px;
  display: flex;
  flex-direction: column;
  border: solid 1px;
}

body {

  max-width: 100%;
  padding: 30px;
}

@media only screen and (max-width: 768px) {
  #app {
    padding: 5px;
  }
  body {
    margin: 10px;
    padding: 0;
  }
}

.container {
  margin-top: 300px;
  display: flex;
  padding: 40px;
}

.subcontainer {
  margin-bottom: 40px;
}
</style>
