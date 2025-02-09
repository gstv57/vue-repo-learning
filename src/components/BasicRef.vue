<script setup>
import { onMounted, ref } from 'vue'
const myRef = ref('gstv')

onMounted(() => {
  myRef.value.focus()
})
</script>
<template>
  <div>
    <input type="text" placeholder="Enter your name" ref="myRef" />
  </div>
</template>
