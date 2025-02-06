<script setup>
import { computed, ref } from 'vue'

const counter = ref(0)
const squaredCounter = computed(() => counter.value ** 2)

const incrementCounter = () => {
  counter.value++
}
</script>

<template>
  <h1>Counter : {{ counter }}</h1>
  <h1>Squared Cunter : {{ squaredCounter }}</h1>
  <button @click="incrementCounter">+</button>
</template>
