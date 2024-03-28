<script setup lang="ts">
const scores_grouped = [
  [20, 40, 60],
  [19, 38, 57],
  [18, 36, 54],
  [17, 34, 51],
  [16, 32, 48],
  [15, 30, 45]
]
</script>

<template>
  <div class="flex-1 flex flex-col border border-black">
    <div class="flex flex-row">
      <button class="p-4 basis-2/6 grow border border-slate-500">Next Player</button>
      <button class="text-center grow basis-1/6 border border-slate-500">MISS</button>
      <button class="basis-1/6 grow border border-slate-500">Undo</button>
      <button class="basis-1/6 grow border border-slate-500">Bull</button>
      <button class="basis-1/6 grow border border-slate-500">..Bull..</button>
    </div>
    <div class="flex-1 grid grid-cols-3">
      <template v-for="(scores, index) in scores_grouped" :key="index">
        <button
          class="grow border border-slate-500"
          v-for="(score, index) in scores"
          :key="index"
          :value="score"
        >
          {{ score }}
        </button>
      </template>
    </div>
  </div>
</template>
