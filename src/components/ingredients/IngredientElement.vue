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
      <label class="inline-flex items-center">
        <input type="checkbox" class="form-checkbox" checked />
        <span class="ml-2" v-html="ingredient">{{ ingredient }}</span>
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
