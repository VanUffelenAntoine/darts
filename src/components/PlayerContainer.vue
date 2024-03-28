<script setup lang="ts">
defineProps<{
  player: { name: String; score: Number; marks: number[] }
}>()
</script>

<template>
  <div class="flex-1 flex flex-col col-span-2">
    <div class="m-4">
      <div class="mx-auto text-center">{{ player.score }}</div>
      <div class="mx-auto text-center">{{ player.name }}</div>
    </div>

    <div class="flex flex-1 flex-col flex-grow divide-y divide-gray-950 border-y border-y-gray-950">
      <div
        class="grow flex justify-center items-center"
        v-for="(mark, index) in player.marks"
        :key="index"
      >
        <div>{{ mark }}</div>
      </div>
    </div>
  </div>
</template>
