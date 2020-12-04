<template>
  <div class="container">
    <div class="text-container">
      <h1 class="slideInLeft">Build future</h1>
      <h1 class="slideInRight">Build web</h1>
      <h2>Leonardo Mendoza</h2>
      <h3>Software developer</h3>
      <ul>
        <li>More than 5 years working with web technologies</li>
        <li>Working experience with Angular since its release in 2016</li>
        <li>
          Coding practices to build high-performance applications
        </li>
      </ul>

      <div>
        <Button :text="'HIRE ON UPWORK'" />
      </div>
    </div>
    <div class="illustration-container">
      <PlanetIllustration class="planet" />
      <!-- <OrbitIllustration class="orbit" /> -->
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Button from "../components/Button-component.vue";
import PlanetIllustration from "../illustrations/Platnet-illustration.vue";
import OrbitIllustration from "../illustrations/Orbit-iIlustration.vue";

export default defineComponent({
  name: "HelloWorld",
  components: {
    Button,
    PlanetIllustration,
    // OrbitIllustration,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../styles/styles.scss";
@import "../styles/animations.scss";

.orbit {
  top: 0;
  width: 50%;
  z-index: -50;
  top: 0;
  right: -200px;
  opacity: 0.4;
}

.planet {
  transform: scale(1.3) translate(25px, 67px);
  overflow: overlay;
}

.text-container,
.illustration-container {
  width: 40%;
  display: flex;
  flex-direction: column;
}
.text-container {
  width: 60%;
  justify-content: center;
}

button {
  margin-left: 20px;
}

@media only screen and (max-width: 1024px) {
  button {
    margin: 0px;
    margin-top: 15px;
  }
  .planet {
    transform: none;
    z-index: -20;
    opacity: 0.4;
    /* transform: translateY(-256px); */
    position: absolute;
    top: 246px;
  }
}

.container {
  margin-top: 0px;
}

ul {
  padding-left: 25px;

  // list-style-type: none;
}

li,
h2,
h3 {
  margin-top: 15px;
}

@media only screen and (max-width: 1024px) {
  .container {
    padding: 0;
    padding-top: 40px;
    flex-direction: column;
  }
  .text-container,
  .illustration-container {
    width: 100%;
    align-items: center;
    text-align: center;
    li {
      list-style-type: none;
    }
  }
}
</style>
