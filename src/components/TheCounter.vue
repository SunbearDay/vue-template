<script setup>
import { useCounterStore } from "@/stores/counter.js"

const counter = useCounterStore()
</script>

<template>
  <div class="the-counter">
    <article>
      <p>Counter Value: {{ counter.count }}</p>
      <p>Get Double Count: {{ counter.doubleCount }}</p>
      <button @click="counter.increment">Increment Counter</button>
    </article>
  </div>
</template>

<style scoped>
article {
  display: grid;
  gap: 1rem;
  justify-content: start;
  margin-block: 2rem;
}
</style>