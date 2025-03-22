<script setup>
import { RouterView, RouterLink } from "vue-router";
</script>

<template>
  <div class="container">
    <header>
      <h1>Contact Book</h1>
      <nav>
        <RouterLink to="/">Home</RouterLink> |
        <RouterLink to="/add">Add Contact</RouterLink>
      </nav>
    </header>

    <RouterView />
  </div>
</template>

<style scoped>
.container {
  text-align: center;
  font-family: Arial, sans-serif;
}
</style>
