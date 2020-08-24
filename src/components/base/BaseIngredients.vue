<template>
  <div class="w-2/4">
    <h2 class="playfair-display font-bold text-2xl mb-8">Ingredients</h2>
    <IngredientElement
      v-for="(element, index) in recipeElements"
      :key="index"
      :recipeElement="element"
    ></IngredientElement>
  </div>
</template>

<script>
import IngredientElement from "@/components/ingredients/IngredientElement.vue";
export default {
  components: {
    IngredientElement,
  },
  props: {
    recipeElements: Array,
  },
};
</script>

<style></style>
