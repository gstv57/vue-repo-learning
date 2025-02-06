<script setup>
import { computed, ref } from 'vue'
const firstName = ref('Gustavo')
const lastName = ref('de Moraes')

const fullName = computed(() => firstName.value + ' ' + lastName.value)
</script>

<template>
  <h1>Fullname : {{ fullName }}</h1>
</template>
