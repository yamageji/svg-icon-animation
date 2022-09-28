<script setup lang="ts">
type Emits = {
  (e: 'click'): void;
};

const emit = defineEmits<Emits>();
const handleClick = () => {
  emit('click');
};
</script>

<template>
  <button
    class="group inline-flex items-center gap-2 rounded-full bg-gray-700 px-4 py-1.5 font-semibold text-white hover:bg-gray-900"
    @click="handleClick"
  >
    <slot />
  </button>
</template>
