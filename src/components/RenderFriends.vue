<script setup>
import { ref } from 'vue'
const friends = ref(['Gustavo', 'Henrique', 'de Moraes'])
</script>
<template>
  <div>
    <ul>
      <li v-for="(friend, i) in friends" :key="i">
        {{ friend }}
      </li>
    </ul>
  </div>
</template>
