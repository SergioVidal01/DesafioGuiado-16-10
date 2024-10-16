<template>
    <div class="d-flex justify-content-center">
      <img :src="url" :alt="`Avatar de ${url}`" :width="tamaño" :height="tamaño" class="rounded-circle">
    </div>
  </template>
  
  <script>
  export default {
    name: "Avatar",
    props: {
      url: String,
      tamaño: {
        type: Number,
        required: true,
      },
    },
  };
  </script>