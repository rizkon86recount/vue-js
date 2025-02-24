<script setup>
import { ref } from "vue";

console.info("Load Component");
let count = ref(0);

function increment() {
  console.info(`increment counter : ${count.value}`);
  count.value++;
}
</script>

<template>
  <h1 id="naik">Counter : {{ count }}</h1>
  <button v-on:click="increment">increment</button>
</template>

<style scoped></style>
