<script setup>
const showMessage = (message) => alert(message)
</script>

<template>
  <button @click="showMessage('This is my message')">Show Message</button>
</template>
