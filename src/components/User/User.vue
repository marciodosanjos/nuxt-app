<template>
  <div>
    <form class="form" action="" method="post">
      <label for="name">Nome:</label>
      <input type="text" id="name" name="name" v-model="name" />
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" v-model="email" />
      <input type="text" id="name" name="name" v-model="name" />
      <label for="sobrenome">Sobrenome:</label>
      <input
        type="text"
        id="sobrenome"
        name="sobrenome"
        v-model="person.lastName"
      />
      <label for="birth-date">Nascimento:</label>
      <input
        type="date"
        id="birth-date"
        name="birth-date"
        v-model="person.birthDate"
      />
    </form>
  </div>

  <p>{{ name }}</p>
  <p>{{ email }}</p>
  <p>{{ person.lastName }}</p>
  <p>{{ person.birthDate }}</p>
</template>

<script setup lang="ts">
import {
  ref,
  reactive,
  onMounted,
  onBeforeMount,
  onBeforeUpdate,
  onUpdated,
  onUnmounted,
  onBeforeUnmount,
} from "vue";
import type { User } from "./User.ts";

//usar ref para tipos primitivos
const name = ref<string>("");
const email = ref<string>("");

//usar reative para tipos derivados
const person: User = reactive({
  name: "",
  email: "",
  lastName: "",
  birthDate: "",
});

/* onBeforeMount(() => {
  console.log("onBeforeMount");
}); */

onMounted(() => {
  console.log("onMounted");
});

/* onBeforeUpdate(() => {
  console.log("onBeforeUpdate");
});
onUpdated(() => {
  console.log("onUpdated");
});

onBeforeUnmount(() => {
  console.log("onBeforeUnmount");
});

onUnmounted(() => {
  console.log("onUnmounted");
}); */
</script>

<style scoped>
.form {
  margin: 0 auto;
  padding: 5px;
  width: 200px;
  background-color: antiquewhite;
}
</style>
