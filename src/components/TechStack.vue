<template>
  <div class="container">
    <div class="ilustration-container">
      <TechStackBackIlustration class="tech-stack-background" />

      <TechStackIlustration class="tech-stack" />
    </div>
    <div class="text-container">
      <h2>Love open source</h2>
      <p>
        SampSSamplSample textSample text textaSample texSampSSamplSample
        textSample text textaSample textSamSample textple texSample textSample
        textSample Sample texttexSample tSatSamSample textple texSample
        textSample textSample Sample texttexSample tSample textextxtle
        SamSampSSamplSample textSample text textaSample textSamSample textple
        texSample textSample textSample Sample texttexSample tSaple textSample
        textSample texttext
      </p>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Button from "./Button.vue";
import PlanetIlustration from "./PlatnetIlustration.vue";
import OrbitIlustration from "./OrbitIlustration.vue";
import TechStackIlustration from "./TechStackioIlustration.vue";
import TechStackBackIlustration from "./TechStackBackIlustration.vue";

export default defineComponent({
  name: "TechStack",
  components: { TechStackIlustration, TechStackBackIlustration },
});
</script>

<style scoped lang="scss">
@import "../styles/styles.scss";

.container {
  margin-top: 300px;
  background-color: $base-mid;
  display: flex;
  margin-left: -40px;
  margin-right: -40px;
}

.ilustration-container {
  flex-shrink: 0;
  width: 1200px;
  margin-top: -60px;
  left: 0;
  
}

.ilustration-container > svg {
  position: absolute;
}

.text-container {
  padding: 40px;
  padding-left: 100px;
  height: 600px;
}

.tech-stack {
  margin-top: 40px;
  width: 800px;
  overflow: overlay;
  margin-left: 400px;
}

.tech-stack-background {

  width: 800px;
  margin-left: 200px;
}

@import "../styles/styles.scss";
@import "../styles/animations.scss";
</style>
