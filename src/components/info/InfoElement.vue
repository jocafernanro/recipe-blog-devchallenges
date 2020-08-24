<template>
  <div class="flex flex-row items-center mb-8">
    <i class="material-icons mr-4 text-3xl" :class="element.color">{{
      element.icon
    }}</i>
    <div class="flex flex-col">
      <span class="uppercase text-gray-500 font-bold text-xs">{{
        element.property
      }}</span>
      <span class="text-sm font-medium" :class="element.color">{{
        element.data
      }}</span>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    element: Object,
  },
};
</script>

<style></style>
