<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import LayoutScaffold from './components/LayoutScaffold.vue'
</script>

<template>
  <LayoutScaffold>
    <header>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </header>
    <RouterView />
  </LayoutScaffold>
</template>
