<script setup>
const myMessage = 'Yellow World'
const myNumber = 100

function add(x, y) {
  return x + y
}
</script>

<template>
  <h1>{{ myMessage }}</h1>
  <h1>{{ myNumber }}</h1>
  <h1>{{ add(10, 10) }}</h1>
</template>

<style scoped></style>
