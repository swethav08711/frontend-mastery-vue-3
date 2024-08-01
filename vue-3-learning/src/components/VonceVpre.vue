<template>
  <textarea v-model="data.title" />
  <p v-once>hello {{ data.title }}</p>
  <span v-pre>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nesciunt voluptatem incidunt animi maxime voluptatum eos unde officia neque placeat, delectus facere quibusdam, repudiandae aperiam dolorem! Impedit veritatis ut doloribus distinctio?
  Eum optio, provident, voluptatibus laborum enim nulla esse, suscipit mollitia ipsum porro quaerat quia animi. Quis, dolorem similique iusto voluptas assumenda expedita aperiam reprehenderit explicabo, facere corporis totam suscipit quaerat? {{ data.title  }} </span>
  <pre>{{ data }}</pre>
</template>

<script setup>
import { ref } from "vue";
const data = ref(null);
data.value = {
  title: "Hellow",
};
</script>
