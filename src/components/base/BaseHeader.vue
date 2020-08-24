<template>
  <div class="mb-8">
    <h1 class="playfair-display font-bold text-2xl md:text-5xl mb-4 mt-8">
      {{ name }}
    </h1>
    <div class="flex flex-row">
      <svg
        width="40"
        height="8"
        viewBox="0 0 13 8"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="mr-4"
      >
        <circle cx="1.5" cy="1.5" r="1.5" fill="#C4C4C4" />
        <circle cx="1.5" cy="6.5" r="1.5" fill="#C4C4C4" />
        <circle cx="6.5" cy="1.5" r="1.5" fill="#C4C4C4" />
        <circle cx="6.5" cy="6.5" r="1.5" fill="#C4C4C4" />
        <circle cx="11.5" cy="1.5" r="1.5" fill="#C4C4C4" />
        <circle cx="11.5" cy="6.5" r="1.5" fill="#C4C4C4" />
      </svg>
      <p class="text-sm md:w-2/3 -mt-1 italic">
        {{ description }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name: String,
    description: String,
  },
};
</script>

<style></style>
