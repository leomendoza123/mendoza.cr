<template>
  <h1 class="slideInLeft">Build the future</h1>
  <h1 class="slideInRight">Build web</h1>

  <h2>Leonardo Mendoza</h2>
  <h3>Software developer</h3>
  <ul>
    <li>More than 7 years working with web techonologies</li>
    <li>Working expirience with Angular since it’s release in 2016</li>

    <li>
      Application performance, internationalizaiton and accesibility expert
    </li>
  </ul>

  <Button :text="'HIRE ON UPWORK'" />
  <PlanetIlustration class="planet"></PlanetIlustration>
  <OrbitIlustration class="orbit" />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Button from "./Button.vue";
import PlanetIlustration from "./PlatnetIlustration.vue";
import OrbitIlustration from "./OrbitIlustration.vue";

export default defineComponent({
  name: "HelloWorld",
  components: {
    Button,
    PlanetIlustration,
    OrbitIlustration,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../styles/styles.scss";
@import "../styles/animations.scss";

.orbit {
  position: absolute;
  top: 0;
  width: 50%;
  z-index: -50;
  top: 0;
  right: -200px;
  opacity: 0.4;
}

.planet {
  width: 947px;
  position: absolute;
  top: 40px;
  right: 13%;
  overflow: overlay;
  z-index: -25;
}

button {
  margin: 10px 0 10px 0;
}

ul {
  padding-left: 25px;

  // list-style-type: none;
}
</style>
