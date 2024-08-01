<template>

  <div>
    <textarea v-model="dynamicMessage" />
    <p>{{ dynamicMessage }}</p>
  </div>
  <hr />

  <div>
    <!-- <input type="checkbox" value="vuejs" v-model="checkboxOptions" />
    <label for="vuejs">vuejs</label>
    <input type="checkbox" value="react" v-model="checkboxOptions" />
    <label for="react">react</label>
    <input type="checkbox" value="html" v-model="checkboxOptions" />
    <label for="html">html</label> -->

    <div v-for="option in options" :key="option.name">
      <input type="checkbox" :value="option.name" v-model="checkboxOptions"  :id="option.value"/>
      <label for="option.name">{{ option.name }}</label>
    </div>

    <span>{{ checkboxOptions }}</span>
  </div>
</template>

<script setup>
import { ref } from "vue";
const dynamicMessage = ref(null);
dynamicMessage.value = "Thsi is a mead";

const checkboxOptions = ref([]);
const options = [
  {
    name: "vuejs",
  },
  {
    name: "react",
  },
  {
    name: "html",
  },
];
</script>

<style scoped></style>
