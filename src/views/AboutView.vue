<template>
  <v-card
    class="mx-auto"
    variant="outlined"
  >
  <v-card-item>
    <div>This is about page</div>
  </v-card-item>
  <v-card-actions>
    <v-btn @click="store.increaseCount" 
    class="btn bg-primary"
      variant="outlined">
        {{ store.count }}
    </v-btn>
  </v-card-actions>
  </v-card>
</template>
<script setup lang="ts">
import { useCounterStore } from '@/store/counter';
const store = useCounterStore()
</script>
