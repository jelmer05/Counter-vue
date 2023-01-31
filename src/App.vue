<script setup>
import { ref } from "vue";

const count = ref(0);
</script>
<template>
  <div class="container-fluid container-counter h-100">
    <div class="row header justify-content-center">
      <div class="col-md-10">
        <h1>Counter</h1>
        <h3>{{ count }}</h3>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-md-4">
        <button class="btn btn-lg btn-light" @click="count--">-</button>
        <button class="btn btn-lg btn-light" @click="count++">+</button>
      </div>
    </div>
  </div>
</template>
<style scoped>
.container-counter {
  display: flex;
  justify-content: center;
  flex-direction: column;
}
.header {
  text-align: center;
}
.col-md-4 {
  display: flex;
  justify-content: center;
  gap: 190px;
}
</style>
