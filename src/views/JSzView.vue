<script setup lang="ts">
  import { useCounterStore } from '@/stores/counter';
  const counter = useCounterStore();
</script>


<template>
  <div class="jsz">
    <h1>This is an JSz page</h1>
    <h2>Licznik: {{ counter.count }}</h2>
    <button @click="counter.increment">Kliknij mnie</button>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .jsz {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
