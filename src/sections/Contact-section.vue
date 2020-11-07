<template>
  <div class="container">
    <div class="text-container">
      <h2>Let's get working</h2>

      <Button :text="'HIRE ON UPWORK'" />

      <ContactIllustration />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import ContactIllustration from "../illustrations/Contact-illustration.vue";
import Button from "../components/Button-component.vue";
export default defineComponent({
  name: "Contact",
  components: { ContactIllustration, Button },
});
</script>

<style scoped lang="scss">
@import "../styles/styles.scss";

.container {
  background-color: #414141;
}
.text-container {
  max-width: 1200px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

button {
  margin: 10px 0 10px 0;
  flex-grow: 0;
  max-width: 300px;
}

@import "../styles/styles.scss";
@import "../styles/animations.scss";
</style>
