<script setup>
import { ref } from "vue";

const count = ref(0);
</script>
<template>
  <div>
    <h1>Counter</h1>
    <p>{{ count }}</p>
    <div>
      <button @click="count--">-</button>
      <button @click="count++">+</button>
    </div>
  </div>
</template>
<style scoped>
div {
  height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>
