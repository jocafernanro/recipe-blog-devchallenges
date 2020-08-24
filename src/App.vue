<template>
  <div id="app" class="container mx-auto">
    <BaseHeader></BaseHeader>
    <img src="images/photo1.png" alt="cover" />
    <section class="my-8">
      <BaseIngredients></BaseIngredients>
      <BaseInfo></BaseInfo>
    </section>
    <BaseInstructions></BaseInstructions>
  </div>
</template>

<script>
import BaseHeader from "@/components/base/BaseHeader.vue";
import BaseIngredients from "@/components/base/BaseIngredients.vue";
import BaseInstructions from "@/components/base/BaseInstructions.vue";
import BaseInfo from "@/components/base/BaseInfo.vue";

export default {
  name: "App",
  components: {
    BaseHeader,
    BaseIngredients,
    BaseInstructions,
    BaseInfo,
  },
};
</script>

<style>
:root {
  --global-font-family: "Montserrat", "Helvetica Neue", -apple-system,
    BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif;
  --global-secundary-font-family: "Playfair Display", "Helvetica Neue",
    -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif;
  --global-font-size: 1rem;
  --font-weight-regular: 400;
  --font-weight-bold: 700;
}
html,
body {
  font-family: var(--global-font-family);
  font-size: 16px;
  font-weight: var(--font-weight-regular);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  scroll-behavior: smooth;
  max-width: 1920px;
  margin: 0 auto;
}

.montserrat {
  font-family: var(--global-font-family);
}

.playfair-display {
  font-family: var(--global-secundary-font-family);
}
</style>
