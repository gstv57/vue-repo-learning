<script setup>
import FromComponent from './components/FromComponent.vue'

const formHandler = (username, email, password) => {
  console.log(username, email, password)
}
</script>

<template>
  <FromComponent @userInfo="formHandler" />
</template>
