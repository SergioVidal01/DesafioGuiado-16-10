<template>
    <div class="card" style="width: 18rem;">
      <div class="card-body">
        <h5 class="card-title">{{ nombre }}</h5>
        <p class="card-text">{{ descripcion }}</p>
      </div>
    </div>
  </template>
  <script>
  export default {
    name: "Tarjeta",
    props: {
      nombre: String,
      descripcion: String,
    },
  };
  </script>