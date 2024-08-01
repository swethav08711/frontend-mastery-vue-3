<template>
  <textarea v-model="data" />
  <!-- <button v-show="data">Submit</button> -->
  <button v-if="data">Submit</button>
  <button v-else>Not submit</button>
</template>

<script setup>
import { ref } from "vue";
const data = ref(null);
data.value = "";
</script>

<style scoped></style>
