<template>
  <button
    v-on:click="
      navigate('https://www.upwork.com/freelancers/~0159c5b99b9daecc8e')
    "
  >
    {{ text }}
  </button>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Button",
  props: {
    text: String,
  },
  methods: {
    navigate: (location: string) => {
      window.location.href = location;
    },
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../styles/styles.scss";

button {
  font-size: $paragraph;
  background-color: $base-light;
  border-radius: 5px;
  padding: 10px 20px 10px 20px;
  appearance: none;
  box-shadow: 5px 5px 25px rgba(255, 184, 0, 0.25);
  border: none;
  outline: none;
  -webkit-transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1);
  transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1);
  cursor: pointer;
}
buttona:hover,
button:focus {
  // -webkit-transform: scale(1.05, 1.05);
  // transform: scale(.95, .95);
  box-shadow: 1px 1px 25px rgba(255, 184, 0, 0.25);
}

button:active {
  transform: scale(0.96, 0.96);
  box-shadow: none;
}
</style>
