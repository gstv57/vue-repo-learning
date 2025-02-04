<script setup>
import { reactive } from 'vue'

let initialState = reactive({
  val: {
    count: 0,
  },
  user: ['Gustavo', 'Henrique'],
})

const changeUser = () => {
  initialState.user[0] = 'de Moraes'
  initialState.user[1] = 'Gustavo'
}
</script>

<template>
  <h1>Current count: {{ initialState.val.count }}</h1>
  <h2>Users: {{ initialState.user }}</h2>

  <br />
  <button @click="initialState.val.count += 10">Add 10</button>
  <button @click="changeUser">Change User</button>
  <button @click="initialState.user.push('John Doe')">Add One More</button>
</template>
