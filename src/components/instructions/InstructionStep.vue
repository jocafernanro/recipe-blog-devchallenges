<template>
  <li class="flex flex-row mb-10">
    <div class="">
      <div
        class="playfair-display h-12 w-12 pb-2 text-2xl font-bold  text-white flex flex-row justify-center items-center bg-orange-500 rounded-lg mr-4"
      >
        {{ this.$vnode.key + 1 }}
      </div>
    </div>
    <span class="w-full text-md" v-html="step">{{ step }}</span>
  </li>
</template>

<script>
export default {
  props: {
    step: String,
  },
};
</script>

<style></style>
