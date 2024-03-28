<script setup lang="ts">
import PlayerContainer from '../components/PlayerContainer.vue'

const players = [
  { name: 'Player 1', score: 142, marks: [0, 0, 0, 0, 0, 0] },
  { name: 'Player 1', score: 142, marks: [0, 0, 0, 0, 0, 0] },
  { name: 'Player 1', score: 142, marks: [0, 0, 0, 0, 0, 0] },
  { name: 'Player 1', score: 142, marks: [0, 0, 0, 0, 0, 0] },
  { name: 'Player 1', score: 142, marks: [0, 0, 0, 0, 0, 0] }
]
</script>
<template>
  <div class="flex flex-row divide-x divide-white overflow-scroll border-t border-black">
    <PlayerContainer v-for="(player, index) in players" :key="index" :player="player" />
  </div>
</template>
