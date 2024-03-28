<script setup lang="ts">
import PlayerContainer from '../components/PlayerContainer.vue'
const player = { name: 'Player 1', score: 142, marks: [0, 0, 0, 0, 0, 0] }
</script>
<template>
  <div class="about min-h-full flex flex-col flex-1">
    <PlayerContainer :player="player" />
  </div>
</template>
