<template>
  <header>
    <h1 class="title">{{ projeto }}</h1>
  </header>
</template>

<script setup lang="ts">
const projeto: string = "My nuxt App";
</script>

<style scoped>
.title {
  margin: 0 auto;
  text-align: center;
  color: black;
}
</style>
