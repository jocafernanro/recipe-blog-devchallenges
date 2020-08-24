<template>
  <div>
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
  data: function() {
    return {
      recipeElements: [
        {
          name: "Graham Cracker Crust",
          ingredients: [
            "1 and 1/2cups (150g) <strong>graham cracker crumbs</strong> (about 10 full sheet graham crackers)",
            "5 Tablespoons (70g) <strong>unsalted butter</strong>, melted",
            "1/4 cup (50g) <strong>granulated sugar</strong>",
          ],
        },
        {
          name: "Cheesecake",
          ingredients: [
            "for 8-ounce blocks (904g) full-fat <strong>cream cheese</strong>, softened to room temperature",
            "1 cup (200g) <strong>granulated sugar</strong>",
            "1 cup (240g) full-fat <strong>sour cream</strong>, at room temperature",
            "1 teaspoon <strong>pure vanilla extract</strong>",
            "2 teaspoons <strong>fresh lemon juice</strong> (optional, but recommended)",
            "3 large <strong>eggs</strong>, at room temperature",
            "topping suggestions: <i>salted caramel, lemmon curd, strawberry topping, chocolate ganache, red wine chocolate ganache, fresh fruit, whupped cream, or raspberry sauce (recipe in notes)</i>",
          ],
        },
      ],
    };
  },
};
</script>

<style></style>
