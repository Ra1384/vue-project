
<template>
  <div class="counter">
    <h1>شمارنده من</h1>

    <div class="count">{{ count }}</div>

    <div class="buttons">
      <button @click="count++"> +</button>

      <button @click="count--"> -</button>

      <button @click="count = 0">بازنشانی</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<style>
.counter {
  direction: rtl;
  text-align: center;
  font-family: Tahoma, sans-serif;
  margin: 100px auto;
  padding: 30px;
  max-width: 400px;
  background-color: #f5e6d3;
  border-radius: 20px;
}

h1 {
  color: #432319;
}

.count {
  font-size: 60px;
  font-weight: bold;
  color: #80502d;
  margin: 25px;
}

.buttons {
  display: flex;
  justify-content: center;
  gap: 10px;
  flex-wrap: wrap;
}

button {
  padding: 12px 18px;
  border: none;
  border-radius: 10px;
  background-color: #80502d;
  color: white;
  cursor: pointer;
  font-size: 14px;
}

button:hover {
  background-color: #432319;
}
</style>
