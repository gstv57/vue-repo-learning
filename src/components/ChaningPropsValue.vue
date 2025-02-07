<script setup>
const props = defineProps(['myFavoriteNumber'])
// props.myFavoriteNumber = 10  ❌❌
// Props are "immutable" which means there value cannot be changed
// -- and they're just readonly
</script>

<template>
  <h1>{{ props.myFavoriteNumber }}</h1>
</template>
