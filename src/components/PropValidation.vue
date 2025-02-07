<script setup>
// Basic Validation
// const props = defineProps({
//   fullName: String,
//   age: Number,
// })

// Complex Props Validation
const props = defineProps({
  fullName: {
    type: String,
    default: 'Anonymous',
  },
  age: {
    type: Number,
    required: true,
  },
})
</script>

<template>
  <h1>{{ props.fullName }}</h1>
  <h1>{{ props.age }}</h1>
</template>
