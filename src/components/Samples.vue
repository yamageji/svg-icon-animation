<script setup lang="ts">
import MenuButton from './MenuButton.vue';
import UpdateButton from './UpdateButton.vue';
import Download from './Download.vue';
</script>

<template>
  <h2
    class="text-2xl font-bold text-gray-900 before:inline-block before:h-4 before:w-6 before:rounded-full before:bg-indigo-500"
  >
    button sample
  </h2>

  <div class="mt-2 flex flex-col gap-2">
    <div class="mt-4">
      <MenuButton />
    </div>

    <div class="mt-4">
      <UpdateButton />
    </div>

    <div class="mt-4">
      <Download />
    </div>
  </div>
</template>
