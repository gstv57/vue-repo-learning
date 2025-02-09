<script setup>
import { ref } from 'vue'
import ComponentOne from './components/ComponentOne.vue'
import ComponentThree from './components/ComponentThree.vue'
import ComponentTwo from './components/ComponentTwo.vue'

const currentTab = ref('ComponentOne')

const tabs = {
  ComponentOne,
  ComponentTwo,
  ComponentThree,
}
</script>

<template>
  <button @click="currentTab = 'ComponentOne'">1</button>
  <button @click="currentTab = 'ComponentTwo'">2</button>
  <button @click="currentTab = 'ComponentThree'">3</button>
  <hr />
  <component :is="tabs[currentTab]" />
</template>
