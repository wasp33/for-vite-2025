<script setup>
import { ref } from 'vue';

const num =ref(0);
function onClick() {
  num.value += 1;
}

</script>

<template>
  <div>
    <h1>Hello Vite!</h1>
    <button type="button" v-on:click="onClick"> Click Me </button>
    <p>Button clicked {{ num }} times.</p>
  </div>
  
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
