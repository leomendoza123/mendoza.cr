<template>
  <svg
    id="orbit"
    data-name="Layer 1"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 739.14 737.69"
  >
    <defs></defs>
    <path
      class="cls-1"
      d="M620.41,490.86"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-1"
      d="M620.41,820.07"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-2"
      d="M313.73,411c21.1,170.17,154.66,305.47,324,329.21"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-1"
      d="M725.42,419.44"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-1"
      d="M725.42,748.65"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-2"
      d="M1049.42,419.44c-21.1,170.17-154.66,305.47-324,329.21"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-1"
      d="M726.19,341.16"
      transform="translate(-311.54 -11.45)"
    />
    <path class="cls-1" d="M726.19,12" transform="translate(-311.54 -11.45)" />
    <path
      class="cls-2"
      d="M1050.19,341.16C1029.08,171,895.53,35.69,726.19,12"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-1"
      d="M1063.67,843.49"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-1"
      d="M860.68,721.26"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-1"
      d="M860.68,392.05"
      transform="translate(-311.54 -11.45)"
    />
    <path
      class="cls-2"
      d="M312,343.07C333.15,172.9,466.7,37.6,636,13.86"
      transform="translate(-311.54 -11.45)"
    />
  </svg>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "OrbitIlustration",
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../styles/animations.scss";

svg#orbit {
  animation: spin 10s linear infinite;
}

.cls-1 {
  fill: #fff;
}
.cls-1,
.cls-2 {
  stroke: #fff;
  stroke-miterlimit: 10;
}
.cls-2 {
  fill: none;
}
</style>
