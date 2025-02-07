<script setup>
// Basic Validation
const props = defineProps({
  fullName: String,
  age: Number,
})
</script>

<template>
  <h1>{{ props.fullName }}</h1>
  <h1>{{ props.age }}</h1>
</template>
