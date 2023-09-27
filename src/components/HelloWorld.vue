<script setup lang="ts">
import { useCounterStore } from '../stores/counter';
const store = useCounterStore();
</script>

<template>
  From HelloWorld:
  <div class="card">
    {{ store.doubleCount }}
    <button type="button" @click="store.increment">
      count is {{ store.count }}
    </button>
  </div>
</template>
