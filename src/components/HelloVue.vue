<script setup>
console.info("Hello Vue");

const hello = "<h1>Hello Vue</h1>";
const data = {
  class: "hello",
  id: "hello",
};
const buttonDisabled = false;
function helloFunction() {
  return "Hello Rizkon Ganteng";
}
</script>

<template>
  <h1 v-bind="data">{{ hello.toUpperCase() }}</h1>
  <h2>{{ 100 * 200 }}</h2>
  <div :class="data.class" v-html="hello"></div>
  <h2>{{ helloFunction() }}</h2>

  <button :disabled="buttonDisabled">This is button</button>
</template>

<style scoped>
.hello {
  color: green;
}
</style>
