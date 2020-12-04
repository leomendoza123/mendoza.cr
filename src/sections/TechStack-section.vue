<template>
  <div class="container">
    <div class="ilustration-container">
      <div class="ilustration-inner-container">
        <TechStackIllustration class="tech-stack" />
      </div>
    </div>
    <div class="text-container">
      <div class="subcontainer">
        <h4>🛠️My tech stack</h4>
        <p>
          Over 5 years of experience working on projects used by millions. With
          a deep passion for the details and attention for every line of code, I
          have acquired bast knowledge on the following technologies.
        </p>
        <p>
          <strong>
            Javascript, Typescript, Angular, Angular Components, RxJS, Webpack,
            Cypress, Html, SCSS, CSS, Git.
          </strong>
        </p>
      </div>
      <div class="subcontainer">
        <h4>📚Areas of expertise</h4>
        <p>
          Making SPA(simple single-page applications) and PWA (progressive web
          apps) applying and bringing awareness to the web development best
          practices.
        </p>
        <h5>Architecture, performance, and scalability</h5>
        <p>
          I design carefully designed front-end architectures that are well
          thought, highly optimized, and modularized to be smoothly served to
          the end-users. Always looking to having great performance and a great
          user experience.
        </p>
        <h5>Code practices</h5>
        <p>
          My code is my passion, that is why I take great pride in building
          easy-to-read highly maintainable code with a strong emphasis on OOP
          (Object-oriented programming), componentization, and well-planned
          styling systems. All this not only contributes to the immediate goals
          of the projects but also to enable a long-lasting product life.
        </p>

        <h5>Frontend cross-platform and inclusivity</h5>
        <p>
          I have a trajectory working with applications that require web
          accessibility and internationalization. To serve every kind of user
          across the world consuming the content from every type of browser and
          device.
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
  margin-top: 35px;
}

h4,
h5 {
  margin-bottom: 10px;
}

.container {
  margin-top: 100px;
  background-color: $base-mid;
  display: flex;
  margin-left: -40px;
  margin-right: -40px;
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
