<script setup>
defineProps({
  type: {
    type: String,
    default: 'button',
  },
  disabled: {
    type: Boolean,
    default: false,
  },
});
</script>

<template>
  <button
      :type="type"
      :disabled="disabled"
      class="inline-flex items-center rounded-md border border-transparent  bg-indigo-600 hover:bg-indigo-700 px-4 py-2 text-xs font-semibold uppercase tracking-widest text-white transition duration-150 ease-in-out  focus:bg-indigo-800 focus:outline-none
        active:bg-indigo-900"    >
    <slot />
  </button>
</template>