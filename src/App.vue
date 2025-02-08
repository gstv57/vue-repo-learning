<script setup>
import SlotComponent from './components/SlotComponent.vue'
import FallbackContent from './components/FallbackContent.vue'
import NomedSlot from './components/NomedSlot.vue'
</script>

<template>
  <SlotComponent>
    <h1>Content</h1>
    <h2>Content</h2>
  </SlotComponent>
  <hr />
  <FallbackContent> </FallbackContent>
  <hr />
  <NomedSlot>
    <template v-slot:one> <h1>one</h1> </template>
    <template v-slot:two> <h2>two</h2></template>
  </NomedSlot>
  <hr />
</template>
