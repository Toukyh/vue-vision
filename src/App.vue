<template>
  <div class="flex justify-between items-center gap-2">
    <button class="p-3 bg-red-600 rounded-md text-white" @click="store.decrement()">-</button>
    <div class="text-white font-semibold text-xl">
      count :
      {{ store.count }}
    </div>
    <button class="p-3 bg-green-600 rounded-md text-white" @click="store.increment()">+</button>
  </div>
</template>
<script setup lang="ts">
import { useCounterStore } from './stores/counter'

const store = useCounterStore()
</script>
