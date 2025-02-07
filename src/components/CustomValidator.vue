<script setup>
defineProps({
  name: {
    type: String,
    validator: (propValue) => {
      return ['Gustavo', 'Henrique', 'de Moraes'].includes(propValue)
    },
  },
  age: {
    type: Number,
    validator: (propValue) => (propValue >= 8 && propValue <= 30 ? true : false),
  },
  password: {
    type: String,
    validator: (propValue) => propValue.length >= 8,
  },
})
</script>

<template>
  <h1>Name: {{ name }}</h1>
  <hr />
  <h1>Age: {{ age }}</h1>
  <hr />
  <h1>Password: {{ password }}</h1>
  <hr />
</template>
