<script setup lang="ts">
import { ref } from 'vue';
import { RouterLink, RouterView } from 'vue-router';
const hue = ref(210);
</script>

<template>
  <div class="wrapper">
    <header>
      <nav class="flex gap-2 items-center justify-center">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/week">Week</RouterLink>
      </nav>
      <div class="flex gap-2 items-center justify-center">
        <input
          v-model="hue"
          type="range"
          min="0"
          max="360" />
        {{ hue }}
      </div>
    </header>

    <RouterView />
  </div>
</template>

<style scoped>
.wrapper {
  --hue: v-bind(hue);
}
</style>
