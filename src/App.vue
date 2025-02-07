<script setup>
import { ref } from 'vue'
import DynamicPropsComponent from './components/DynamicPropsComponent.vue'
import StaticPropsComponent from './components/StaticPropsComponent.vue'

const firstName = ref('Gustavo')
const lastName = ref('de Moraes')
</script>

<template>
  <StaticPropsComponent name="Gustavo" />
  <hr />
  <DynamicPropsComponent :firstName="firstName" :lastName="lastName" />
  <hr />
</template>
