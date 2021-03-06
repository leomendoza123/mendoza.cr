<template>
  <div class="container">
    <div class="ilustration-container">
      <div class="ilustration-inner-container">
        <TechStackIllustration class="tech-stack" />
      </div>
    </div>
    <div class="text-container">
      <div class="subcontainer">
        <h4>🛠️My toolset</h4>
        <p>
          <strong>
            Javascript, Typescript, Angular, Angular Components, RxJS, Webpack,
            Cypress, Html, SCSS, CSS, Git.
          </strong>
        </p>
      </div>
      <div class="subcontainer">
        <h4>📚Areas of expertise</h4>
        <h5>Architecture, performance, and scalability</h5>
        <p>
          I work to have carefully designed
          <strong> front-end architectures </strong> that are well thought,
          highly <strong>optimized</strong> and <strong>modularized</strong> to
          be smoothly served to the end-users. Always looking to having high
          <strong>performance</strong> and a great
          <strong>user experience</strong>.
        </p>
        <h5>Code practices</h5>
        <p>
          My code is my passion, that is why I take great pride in building
          <strong>easy-to-read</strong> highly
          <strong>maintainable</strong> code with a strong emphasis on
          <strong>OOP</strong> (Object-oriented programming),
          <strong>componentization</strong>, and well-planned
          <strong>styling systems</strong>. All this not only contributes to the
          immediate goals of the projects but also to enable a long-lasting
          product life.
        </p>

        <h5>Inclusivity</h5>
        <p>
          I have a trajectory working with
          <strong>cross-platform</strong> applications that require web
          <strong>accessibility</strong> and
          <strong>internationalization</strong>, in this way I have served all
          kinds of users across the world.
        </p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Button from "./Button.vue";
import PlanetIlustration from "./PlatnetIlustration.vue";
import OrbitIlustration from "./OrbitIlustration.vue";
import TechStackIllustration from "../illustrations/TechStack-illustration.vue";

export default defineComponent({
  name: "TechStack",
  components: { TechStackIllustration },
});
</script>

<style scoped lang="scss">
@import "../styles/styles.scss";

h5 {
  margin-top: 10px;
}

h4,
h5 {
  margin-bottom: 10px;
}

.container {
  margin-top: 100px;
  background-color: $base-mid;
  display: flex;
  overflow: hidden;
}

.ilustration-container {
  width: 50%;
  flex-shrink: 0;
}

.text-container {
  max-width: 500px;
}

@media only screen and (max-width: 1024px) {
  .container {
    flex-direction: column-reverse;
    align-items: center;
  }
  .ilustration-container {
    width: 100%;
    flex-shrink: 0;
  }
}

@import "../styles/styles.scss";
@import "../styles/animations.scss";
</style>
