<script setup>
import { ref } from 'vue'
const isVisible = ref(true)
</script>

<template>
  <div v-show="isVisible">
    <p>
      This paragraph will be shown or hidden based on the value on
      <span style="color: blue">isVisible</span>
    </p>
  </div>
  <button @click="isVisible = !isVisible">Toggle</button>
</template>
