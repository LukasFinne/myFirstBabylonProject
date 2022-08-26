<template>
  <div>
    <h3>Babylons Examples</h3>
    <canvas></canvas>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { StandardMaterials } from "@/BabylonsExamples/StandardMaterials";
export default defineComponent({
  name: "BabylonsExamples",
  mounted() {
    const canvas = document.querySelector("canvas")!;
    new StandardMaterials(canvas);
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
canvas {
  width: 70%;
  height: 70%;
}
</style>
