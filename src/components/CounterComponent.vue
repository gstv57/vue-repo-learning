<script setup>
import { useCounter } from '../shared/useCounter'

const counter = useCounter()
</script>
<template>
  <h1>Count : {{ counter.count }}</h1>
  <button @click="counter.increment">Incrememt</button>
  <button @click="counter.decrement">Decrememt</button>
</template>
