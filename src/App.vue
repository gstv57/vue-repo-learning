<script setup>
import SlotComponent from './components/SlotComponent.vue'
import FallbackContent from './components/FallbackContent.vue'
</script>

<template>
  <SlotComponent>
    <h1>Content</h1>
    <h2>Content</h2>
  </SlotComponent>
  <hr />
  <FallbackContent> </FallbackContent>
</template>
