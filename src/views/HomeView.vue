<script setup lang="ts">
import { useCounterStore } from '@/store/counter';
const store = useCounterStore()
</script>

<template>
  <v-card
  class="mx-auto"
  variant="outlined">
  <v-card-item>
    {{ store.count }}
  </v-card-item>
  <v-card-item>
    <v-chip class="ma-2"
    color="primary">
      count is : {{ store.oddOrEven }}
    </v-chip>
  </v-card-item>
  <v-card-actions>
    <v-btn @click="store.decreaseCount" 
      class="btn bg-error">
        -
    </v-btn><v-spacer/>
    <v-btn @click="store.increaseCount" 
      class="btn bg-secondary"
      variant="outlined">
        +
    </v-btn>
  </v-card-actions>
  </v-card>
</template>

<style>
  div {
    margin: 50px;
    font-size: 50px;
  }
  v-btn {
    width: 100px;
    font-size: 50px;
    margin-left: 50px;
  }
</style>
