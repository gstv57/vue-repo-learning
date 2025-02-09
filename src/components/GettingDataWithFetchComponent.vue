<script setup>
import { ref } from 'vue'

const data = ref(null)

const fetchData = () => {
  fetch('https://jsonplaceholder.typicode.com/posts')
    .then((response) => {
      if (!response.ok) {
        throw new Error('HTTP Error! Status: ${response.status}')
      }
      return response.json()
    })
    .then((responseData) => {
      data.value = responseData
    })
    .catch((err) => {
      console.log(err)
    })
}
</script>
<template>
  <div>
    <h1>(( using Fetch))</h1>
    <button @click="fetchData">Fetch Data</button>
  </div>
  <div>
    <div>
      <h2>Data from API:</h2>
      <ul v-for="{ id, title, body } in data" :key="id">
        <li>ID: {{ id }}</li>
        <li>Title: {{ title }}</li>
        <li>Body: {{ body }}</li>
      </ul>
    </div>
  </div>
</template>
