<script setup>
import { ref } from 'vue'
let books = ref([
  ['The Great Gatsby', 'F. Scott Fitzgerald'],
  ['The Catcher in the Rye', 'J.D. Salinger'],
  ['To Kill a Mockingbird'],
  ['1984', 'George Orwell', 'Dystopian'],
  ['Pride and Prejudice', 'Jane Austen'],
  ['Wuthering Heights', 'Emily Bronte'],
  ['Jane Eyre', 'Charlotte Bronte'],
  ['Moby-D'],
])
</script>

<template>
  <ul v-for="(book, i) in books" :key="i">
    <li v-for="(b, index) in book" :key="index">
      {{ b }}
    </li>
  </ul>
</template>
