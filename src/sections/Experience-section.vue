<template>
  <div class="container">
    <div class="text-container">
      <h3>Recent experience</h3>
      <div class="subcontainer">
        <h5>💚 orcid.org</h5>
        <h6><strong>Front End Developer</strong></h6>

        <h6>2018 - to the present</h6>
        <h6>Full remote</h6>
        <p>
          Currently leading a complete front-end migration from a monolithic
          project into a microservice <strong>Angular</strong> based project.
          Consumed by <strong>over a million unique users every week</strong>,
          translated into <strong>12 languages</strong> including Arabic (yes
          right to left display!), <strong>accessible</strong>, architected to
          have <strong>great performance</strong>, highly
          <strong>maintainable</strong>, <strong>scalable</strong>, and is 100%
          <strong>open source</strong>.
        </p>

        <p>
          Also participating in the implementation of a fully
          <strong>tested and automatized continuous integration</strong>
          and delivery process.
        </p>

        <p>
          Here I work with other developers, designers, tech support, and
          product owners, using a canvas methodology.
        </p>
      </div>

      <div class="subcontainer">
        <h5>👨‍🍳 pamperedchef.com</h5>
        <h6><strong>Full Stack Developer</strong></h6>
        <h6>Mar 2018 - Sep 2020</h6>
        <h6>Full remote</h6>
        <p>
          Worked on the migration of a web shopping cart from a monolithic
          java-based frontend into an Angular app. Consumed by over
          <strong>3 million daily users</strong>, accessible and build to have
          great performance.
        </p>
        <p>
          There I worked with an agile <strong>scrum</strong> methodology,
          <strong>tested and automated</strong> CI/CD process, and participating
          on one of the 5 technical teams alongside designers and scrum members.
        </p>
      </div>
      <div class="subcontainer">
        <h5>🧪 Previous experience</h5>
        <h6>Mar 2015 - Sep 2018</h6>
        <p>
          Since 2015 I have been working on multiple web projects featuring the
          build of an <strong>ERP</strong>, the build of an
          <strong>artificial intelligence</strong> frontend application that ran
          deep learning on the edge, and the use of
          <strong>web charts </strong> to display geographical data.
        </p>
      </div>
    </div>

    <div class="portrait-container">
      <PortraitIllustration />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import PortraitIllustration from "../illustrations/Portrait-illustration.vue";
export default defineComponent({
  name: "Experience",
  components: { PortraitIllustration },
});
</script>

<style scoped lang="scss">
@import "../styles/styles.scss";

h5 {
  margin-bottom: 20px;
}
h6 {
  margin-bottom: 5px;
}

p {
  margin-top: 10px;
}

.container {
  display: flex;
  justify-content: flex-end;
}

.text-container {
  max-width: 700px;
  flex-grow: 0;
  padding-right: 20px;
}

.portrait-container {
  flex-shrink: 0;
  display: flex;
  justify-content: center;
}

@media only screen and (max-width: 1024px) {
  .container {
    flex-direction: column;
  }
  .ilustration-container {
    width: 100%;
    flex-shrink: 0;
  }
}

@import "../styles/styles.scss";
@import "../styles/animations.scss";
</style>
