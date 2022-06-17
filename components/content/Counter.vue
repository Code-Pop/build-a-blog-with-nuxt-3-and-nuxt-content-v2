<script setup>
const currentCount = ref(0)

const incrementCount = () => {
  currentCount.value += 2
}
</script>

<template>
  <div class="counter">
    <p class="current-count">
      Current Count: <strong>{{ currentCount }}</strong>
    </p>
    <button @click="incrementCount">Add 1</button>
  </div>
</template>

<style>
.counter {
  max-width: 500px;
  padding: 15px;
  margin: 0 auto;
  border: 3px solid #ccc;
  text-align: center;
}

.counter .current-count {
  margin-bottom: 10px;
  text-align: center;
  font-size: 1.5rem;
}

.counter button {
  font-size: 1rem;
  padding: 5px;
}
</style>
