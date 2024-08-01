<template>
  <textarea v-model="content" />
  <button :class="[content ? shoeBtn : '']">Submit</button>
</template>

<script setup>
import { ref } from "vue";
const shoeBtn = ref(null);
const content = ref(null);
shoeBtn.value = "active";
content.value = "Hellow";
</script>

<style scoped>
button.active {
  background-color: red;
  color: white;
}
</style>
