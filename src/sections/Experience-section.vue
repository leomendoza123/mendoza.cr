<template>
  <div class="container">
    <div class="text-container">
      <h2>Expirience</h2>
      <h3>tEST JOB 1</h3>
      <p>
        asdkjaskdjas daskjd oasikdo askd aosdi asdoias odias oasdkjaskdjas
        daskjd oasikdo askd aosdi asdoias odias odiasod iasdo asodi
        asasdkjaskdjas daskjd oasikdo askd aosdi asdoias odias odiasod iasdo
        asodi asasdkjaskdjas daskjd oasikdo askd aosdi asdoias odias odiasod
        iasdo asodi asasdkjaskdjas daskjd oasikdo askd aosdi asdoias odias
        odiasod iasdo asodi as
      </p>

      <h3>tEST JOB 2</h3>
      <p>
        asdkjaskdjas daskjd oasikdo askd aosdi asdoias odias oasdkjaskdjas
        daskjd oasikdo askd aosdi asdoias odias odiasod iasdo asodi
        asasdkjaskdjas daskjd oasikdo askd aosdi asdoias odias odiasod iasdo
        asodi asasdkjaskdjas daskjd oasikdo askd aosdi asdoias odias odiasod
        iasdo asodi asasdkjaskdjas daskjd oasikdo askd aosdi asdoias odias
        odiasod iasdo asodi as
      </p>
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

.container {
  justify-content: flex-end;
}

.text-container {
  max-width: 900px;
  flex-grow: 0;
}



.portrait-container {
  flex-shrink: 0;
}

@import "../styles/styles.scss";
@import "../styles/animations.scss";
</style>
