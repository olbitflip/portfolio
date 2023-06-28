<script lang="ts">
import { defineComponent } from 'vue';
import { RouterLink } from 'vue-router';
export default defineComponent({})
</script>

<template>
    <nav class="w-full h-16 flex flex-row justify-center items-center shadow drop-shadow-lg bg-white">
        <RouterLink to="/">Home</RouterLink>
    </nav>
</template>