<template>
  <div>
    <h3 class="playfair-display italic text-xl my-8">
      {{ recipeElement.name }}
    </h3>
    <div
      v-for="(ingredient, index) in recipeElement.ingredients"
      :key="index"
      class="mb-2"
    >
      <label class="flex fle-col">
        <input type="checkbox" class="form-checkbox text-orange-500 h-5 w-5" />
        <span class="ml-4 -mt-1 md:text-lg" v-html="ingredient">{{
          ingredient
        }}</span>
      </label>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    recipeElement: Object,
  },
};
</script>

<style></style>
