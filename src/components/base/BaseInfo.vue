<template>
  <div class="w-2/4 flex flex-col">
    <div class="pt-10 pb-4 pl-10 pr-16 shadow-md rounded-lg  self-end">
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
