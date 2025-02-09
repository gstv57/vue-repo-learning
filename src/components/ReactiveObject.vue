<script setup>
import { reactive, watch } from 'vue'
const state = reactive({ username: 'gstv' })

watch(
  () => state.username,
  (newValue, oldValue) => {
    console.log('old value: ', oldValue)
    console.log('new value: ', newValue)
  },
)
</script>
<template>
  <h1>{{ state.username }}</h1>
  <button @click="state.username = 'Gstv'">Change Name</button>
</template>
