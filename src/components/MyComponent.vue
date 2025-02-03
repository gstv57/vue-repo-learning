<script setup>
// const myLink = 'https://www.google.com.br'
// const myImage =
//   'https://plus.unsplash.com/premium_photo-1683910767532-3a25b821f7ae?w=400&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MXx8ZnJlZSUyMGltYWdlc3xlbnwwfHwwfHx8MA%3D%3D'

// const altTextImage = 'Only a random picture'

// const imageWidth = 400
// const imageHeight = 400

// dinamic binding

const imageInfo = {
  src: 'https://plus.unsplash.com/premium_photo-1683910767532-3a25b821f7ae?w=400&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MXx8ZnJlZSUyMGltYWdlc3xlbnwwfHwwfHx8MA%3D%3D',
  alt: 'Only a random picture',
  width: 400,
  height: 400,
}
</script>

<template>
  <!-- <a :href="myLink" target="_blank">Google</a> -->
  <!-- <img :src="myImage" :alt="altTextImage" :width="imageWidth" :height="imageHeight" /> -->
  <img :="imageInfo" />
</template>

<style scoped></style>
