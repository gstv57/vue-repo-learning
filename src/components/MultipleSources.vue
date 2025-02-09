<script setup>
import { ref, watch } from 'vue'
const username = ref('gstv')
const counter = ref(0)

watch([username, counter], (newValue, oldValue) => {
  console.log('Old Value: ', oldValue)
  console.log('New Value: ', newValue)
})
</script>
<template>
  <h1>{{ username }}</h1>
  <h1>{{ counter }}</h1>

  <button @click="username = 'gstv57'">Change Name</button>
  <button @click="counter++">Increment Counter</button>
</template>
