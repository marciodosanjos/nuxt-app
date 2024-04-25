<template>
  <TopHeader />
  <NavBar />
  <User />
</template>

<script setup lang="ts">
import TopHeader from "./src/components/Header/TopHeader.vue";
import NavBar from "./src/components/Navbar/Navbar.vue";
import User from "./src/components/User/User.vue";
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

header {
  line-height: 1.5;
}
</style>
