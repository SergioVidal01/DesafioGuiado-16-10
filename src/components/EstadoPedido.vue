<template>
    <div class="alert" :class="estadoClass" role="alert">
      {{ mensajeEstado }}
    </div>
  </template>
  
  <script>
  export default {
    name: "EstadoPedido",
    props: {
      estado: String,
    },
    computed: {
      mensajeEstado() {
        switch (this.estado) {
          case "enviado":
            return "Tu pedido ha sido enviado.";
          case "pendiente":
            return "Tu pedido está pendiente.";
          case "cancelado":
            return "Tu pedido ha sido cancelado.";
          default:
            return "Estado desconocido.";
        }
      },
      estadoClass() {
        switch (this.estado) {
          case "enviado":
            return "alert-success";
          case "pendiente":
            return "alert-warning";
          case "cancelado":
            return "alert-danger";
          default:
            return "alert-secondary";
        }
      },
    },
  };
  </script>