<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="navbar bg-primary">
    <nav>
      <RouterLink to="/">Home</RouterLink> |
      <RouterLink to="/counter">Counter</RouterLink> |
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style>
nav {
  text-decoration-color: white;
  font-size: 30px;
}
</style>
