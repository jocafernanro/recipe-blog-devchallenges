<template>
  <div class="md:w-3/5">
    <h3 class="playfair-display font-bold text-2xl mb-8">Instructions</h3>
    <ol class="">
      <InstructionStep
        v-for="(step, index) in recipeInstructions"
        :key="index"
        :step="step"
      ></InstructionStep>
    </ol>
  </div>
</template>

<script>
import InstructionStep from "@/components/instructions/InstructionStep.vue";
export default {
  components: {
    InstructionStep,
  },
  props: {
    recipeInstructions: Array,
  },
};
</script>

<style></style>
