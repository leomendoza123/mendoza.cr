<template>
  <div class="container">
    <div class="text-container">
      <div class="subcontainer">
        <h5>💚 orcid.org</h5>
        <h6><strong>Front End Developer</strong></h6>

        <h6>2018-to the present</h6>
        <h6>Full remote</h6>
        <p>
          Currently leading a front-end migration project from a monolithic
          Java-based front-end into a new shiny Angular project. This project is
          consumed by over a million unique users every week, translated into 12
          languages including Arabic (yes right to left display!), accessible,
          architected to have great performance, be highly maintainable and
          scalable, and 100% open source. I am currently also participating in
          the implementation of a tested and automatized continuous integration
          and delivery process.
        </p>

        <p>
          Here I work with other developers, designers, tech support, and
          product owners, using a Canvan methodology.
        </p>
      </div>

      <div class="subcontainer">
        <h5>👨‍🍳 pamperedchef.com</h5>
        <h6><strong>Full Stack Developer</strong></h6>
        <h6>Mar 2018- Sep 2020</h6>
        <h6>Full remote</h6>
        <p>
          I did work on the migration of a web shopping cart from a monolithic
          java-based frontend into an Angular app. Consumed by over 3 million
          daily users, accessible and build to have great performance. Alongside
          a full agile scrum methodology, and fully tested and automated
          continuous integration and delivery process.
        </p>
        <p>
          There I worked 100% remote as a member of one of the 5 technical
          teams, with other designers and scrum members.
        </p>
      </div>
      <div class="subcontainer">
        <h5>🧪 Previous experience</h5>
        <h6>Mar 2015- Sep 2018</h6>
        <p>
          Since 2015 I have been working on multiple web projects, from a
          company ERP to an artificial neural network running on a frontend to
          calculate a shopping card location at a supermarket. 
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
  justify-content: flex-end;
}

.text-container {
  max-width: 400px;
  flex-grow: 0;
}

.portrait-container {
  flex-shrink: 0;
}

@import "../styles/styles.scss";
@import "../styles/animations.scss";
</style>
