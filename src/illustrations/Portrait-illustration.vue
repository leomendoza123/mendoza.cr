<template>
  <div class="portrait-illustrations">
    <img width="400" src="../assets/portrait.jpeg" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "PortraitIllustration",
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../styles/animations.scss";

.portrait-illustrations {
  position: relative;
  width: 454px;
}
img {
  box-shadow: 20px 20px black;
  max-width: 100%;
}
</style>
