<script setup lang="ts">
import PlayersContainer from '../components/PlayersContainer.vue'
import ButtonsContainer from '../components/ButtonsContainer.vue'
</script>

<template>
  <div class="bg-red-950 w-full text-3xl flex justify-between px-3">
    <div>Cut throat</div>
    <div>R1/20</div>
  </div>
  <div>Darts left</div>
  <div class="grid flex-grow">
    <PlayersContainer />
    <div class="col col-span-1 flex flex-1">
      <ButtonsContainer />
    </div>
  </div>
</template>
