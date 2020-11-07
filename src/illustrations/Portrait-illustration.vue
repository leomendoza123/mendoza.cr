<template>
  <div class="portrait-illustrations">
    <svg
      class="back"
      width="394"
      height="611"
      viewBox="0 0 394 611"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <rect
        x="0.419373"
        width="393.581"
        height="610.284"
        fill="#0A0A0A"
        fill-opacity="0.9"
      />
    </svg>

    <div class="middle">
      <img src="../assets/portrait.png" />
    </div>

    <svg
      class="front"
      width="394"
      height="612"
      viewBox="0 0 394 612"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <rect
        y="0.824585"
        width="393.581"
        height="610.284"
        fill="#6D695D"
        fill-opacity="0.4"
      />
    </svg>
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
  width: 700px;
}

.back {
  position: absolute;

  top: 10px;
  right: 10px;
}
.middle {
  position: absolute;

  top: 30px;
  right: 30px;
}
.front {
  position: absolute;

  top: 60px;
  right: 60px;
}
</style>
