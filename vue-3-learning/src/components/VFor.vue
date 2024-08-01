<template>

  <div v-for="(value, key, index) in data" :key="value">
    <p>{{ index }}  {{ key }}  {{ value }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
const data = ref(null);

data.value = {
  name: "John Doe",
  age: 30,
  city: "Bangalroe",
};
</script>

<style scoped></style>
