<script setup>
import SchoolComponent from './components/SchoolComponent.vue'
import { provide } from 'vue'

provide('studentName', 'Gustavo')
provide('studentAge', 24)
provide('studentLocation', ['Sorocaba', 'SP'])
</script>

<template>
  <SchoolComponent />
</template>
