<script setup>
import { ref } from 'vue'
import axios from 'axios'

const data = ref(null)

const fetchData = async () => {
  try {
    const response = await axios.get('https://jsonplaceholder.typicode.com/posts')

    data.value = response.data
  } catch (err) {
    console.log(err)
  }
}
</script>
<template>
  <div>
    <h1>(( using Axios))</h1>
    <button @click="fetchData">Fetch Data</button>
  </div>
  <div>
    <h2>Data from API:</h2>
    <ul v-for="{ id, title, body } in data" :key="id">
      <li>ID: {{ id }}</li>
      <li>Title: {{ title }}</li>
      <li>Body: {{ body }}</li>
    </ul>
  </div>
</template>
