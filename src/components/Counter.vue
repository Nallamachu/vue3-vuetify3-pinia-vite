<template>
    <v-card
  class="mx-auto"
  variant="outlined">
    <v-card-item>Present Count Value: {{ store.count }}</v-card-item>
    <v-text-field type="number" v-model="store.count"/>
  </v-card>
</template>

<script setup lang="ts">
import { useCounterStore } from '@/store/counter';

const store = useCounterStore()
</script>