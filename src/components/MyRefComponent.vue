<script setup>
import { ref } from 'vue'

let usersList = ref(['Gustavo', 'Henrique', 'de Moraes'])
</script>

<template>
  <h1>User List: {{ usersList }}</h1>
  <button @click="usersList.push('John')">Add User</button>
</template>
