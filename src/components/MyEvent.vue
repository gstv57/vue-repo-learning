<script setup>
const submitHandler = (e) => {
  e.preventDefault()
  alert('Valid Credentials')
}
</script>

<template>
  <form @:submit="submitHandler">
    <input type="text" placeholder="Please enter your name" />
    <input type="email" placeholder="Please enter your e-mail" />
    <button type="submit">Submit</button>
  </form>
</template>
