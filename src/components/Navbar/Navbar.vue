<template>
  <nav>
    <ul class="navbar">
      <li><a href="">Home</a></li>
      <li><a href="">Sobre</a></li>
      <li><a href="">Login</a></li>
    </ul>
  </nav>
</template>

<script setup lang="ts"></script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-around;
  gap: 20%;
}

ul {
  text-decoration: none;
  list-style-type: none;
}

ul a {
  text-decoration: none;
  color: black;
}

ul a:hover {
  color: grey;
}
</style>
