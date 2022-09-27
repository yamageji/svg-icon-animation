<script setup lang="ts">
import MenuButton from './MenuButton.vue';
import UpdateButton from './UpdateButton.vue';
import Download from './Download.vue';
import BaseButton from './BaseButton.vue';
import ReadMoreButton from './ReadMoreButton.vue';

const menuEvent = () => console.log('menu!');
const updateEvent = () => console.log('update!');
const downloadEvent = () => console.log('download!');
</script>

<template>
  <h2
    class="text-2xl font-bold text-gray-900 before:inline-block before:h-4 before:w-6 before:rounded-full before:bg-indigo-500"
  >
    button sample
  </h2>

  <div class="justify mt-2 flex flex-col gap-2">
    <div class="mt-4">
      <ReadMoreButton />
    </div>
    <div class="mt-4">
      <BaseButton @click="menuEvent">
        MENU
        <MenuButton />
      </BaseButton>
    </div>

    <div class="mt-4">
      <BaseButton @click="updateEvent">
        Update
        <UpdateButton />
      </BaseButton>
    </div>

    <div class="mt-4">
      <BaseButton @click="downloadEvent">
        Download
        <Download />
      </BaseButton>
    </div>
  </div>
</template>
