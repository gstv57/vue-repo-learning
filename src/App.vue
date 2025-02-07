<script setup>
import { ref } from 'vue'
import DynamicPropsComponent from './components/DynamicPropsComponent.vue'
import StaticPropsComponent from './components/StaticPropsComponent.vue'
import ChaningPropsValue from './components/ChaningPropsValue.vue'
import PropValidation from './components/PropValidation.vue'
import ComplexProps from './components/ComplexProps.vue'
const firstName = ref('Gustavo')
const lastName = ref('de Moraes')

const myFavoriteNumber = ref(7)
</script>

<template>
  <StaticPropsComponent name="Gustavo" />
  <hr />
  <DynamicPropsComponent :firstName="firstName" :lastName="lastName" />
  <hr />
  <ChaningPropsValue :myFavoriteNumber="myFavoriteNumber" />
  <hr />
  <PropValidation :age="24" />
  <hr />
  <ComplexProps
    :friends="['Noveli', 'João do Bife', 'Lelis', 'Duran', 'Marcola', 'Malik']"
    :userInfo="{ name: 'Gustavo', age: 24, location: ['Sorocaba', 'SP'] }"
  />
</template>
