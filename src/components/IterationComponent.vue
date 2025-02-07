<script setup>
import { ref } from 'vue'
let books = ref([
  {
    id: 1,
    title: 'Harry Potter',
    author: 'J.K. Rowling',
    genre: 'Fantasy',
    publicationYear: 1997,
  },
  {
    id: 2,
    title: 'The Lord of the Rings',
    author: 'J.R.R. Tolkien',
    genre: 'Fantasy',
    publicationYear: 1954,
  },
  {
    id: 3,
    title: 'A Song of Ice and Fire',
    author: 'George R.R. Martin',
    genre: 'Fantasy',
    publicationYear: 1996,
  },
  {
    id: 4,
    title: 'The Chronicles of Narnia',
    author: 'C.S. Lewis',
    genre: 'Fantasy',
    publicationYear: 1950,
  },
  {
    id: 5,
    title: "The Hitchhiker's Guide to the Galaxy",
    author: 'Douglas Adams',
    genre: 'Science Fiction',
    publicationYear: 1979,
  },
])
</script>

<template>
  <ul v-for="{ id, title, author, genre, publicationYear } in books" :key="id">
    <li>ID: {{ id }}</li>
    <li>Title: {{ title }}</li>
    <li>Author: {{ author }}</li>
    <li>Genre: {{ genre }}</li>
    <li>Publication Year: {{ publicationYear }}</li>
  </ul>
</template>
