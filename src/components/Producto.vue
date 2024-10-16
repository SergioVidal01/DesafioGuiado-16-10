<template>
    <div class="card" style="width: 18rem;">
      <div class="card-body">
        <h5 class="card-title">{{ nombre }}</h5>
        <p class="card-text">Precio: ${{precio}}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Producto",
    props: {
      nombre: String,
      precio: Number,
    },
  };
  </script>