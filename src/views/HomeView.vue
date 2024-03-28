<script setup lang="ts">
import PlayersContainer from '../components/PlayersContainer.vue'
</script>

<template>
  <div class="bg-red-950 w-full text-3xl flex justify-between px-3">
    <div>Cut throat</div>
    <div>R1/20</div>
  </div>
  <div>Darts left</div>
  <div class="grid grid-cols-2 flex-grow">
    <PlayersContainer />
    <div class="col bg-orange-300">game screen</div>
  </div>
</template>
