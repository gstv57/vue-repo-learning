<script setup>
const myRefFunc = (el) => {
  console.log(el.textContent)
  el.textContent = 'Text changed'
  el.style.color = 'crimson'
}
</script>
<template>
  <div>
    <h1 :ref="myRefFunc">Hello</h1>
  </div>
</template>
