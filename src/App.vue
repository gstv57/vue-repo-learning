<script setup>
import ComponentEvent from './components/ComponentEvent.vue'
import { ref } from 'vue'

let count = ref(0)
</script>

<template>
  <h1>Count: {{ count }}</h1>
  <ComponentEvent @incrementCounter="count++" />
</template>
