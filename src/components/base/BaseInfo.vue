<template>
  <div class="order-first md:order-last w-full md:w-2/5 flex flex-col">
    <div
      class="flex flex-row flex-wrap md:flex-col md:pt-10 w-full md:w-auto pb-4 md:pl-10 md:pr-16 md:shadow-md rounded-lg  self-end"
    >
      <InfoElement
        v-for="(element, index) in recipeInfo"
        :key="index"
        :element="element"
      ></InfoElement>
    </div>
  </div>
</template>

<script>
import InfoElement from "@/components/info/InfoElement.vue";
export default {
  components: {
    InfoElement,
  },
  props: {
    recipeInfo: Array,
  },
};
</script>

<style></style>
