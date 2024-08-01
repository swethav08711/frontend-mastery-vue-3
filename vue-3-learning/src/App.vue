<template>
  <div>
    <h1>v-once v-pre</h1>
    <VonceVpre />
    <h1>v-modal</h1>
    <VModal />
    <h1>v-if v-show v-else</h1>
    <VifVelseVshow />
    <h1>v-bind</h1>
    <VBind />
    <h1>v-for</h1>
    <VFor />
  </div>
</template>
<script setup>
import VModal from "./components/VModal.vue";
import VifVelseVshow from "./components/VifVelseVshow.vue";
import VBind from "./components/VBind.vue";
import VFor from "./components/VFor.vue";
import VonceVpre from "./components/VonceVpre.vue";
</script>
<style scoped></style>
