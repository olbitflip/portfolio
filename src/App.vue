<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <nav>
      <RouterLink to="/">Home</RouterLink>
    </nav>
  </header>
  <div class="flex bg-slate-100 justify-center items-center h-screen w-full">
    <RouterView />
  </div>
</template>

<style>

</style>
