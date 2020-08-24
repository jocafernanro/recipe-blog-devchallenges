<template>
  <div
    class="flex flex-row items-center mb-8 md:w-auto"
    :class="element.property === 'Yields' ? 'w-full flex-shrink-0' : 'w-1/3'"
  >
    <i
      class="material-icons mr-1 md:mr-4 text-lg md:text-3xl"
      :class="element.color"
      >{{ element.icon }}</i
    >
    <div class="flex flex-col">
      <span class="uppercase text-gray-500 font-semibold text-xxs">{{
        element.property
      }}</span>
      <span class="text-xs md:text-sm font-medium" :class="element.color">{{
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
