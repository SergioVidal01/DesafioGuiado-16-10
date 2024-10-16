<template>
  <div class="card" style="width: 18rem;">
    <div class="card-body">
      <h5 class="card-title">{{ usuario.nombre }} {{ usuario.apellido }}</h5>
      <p class="card-text">Edad: {{ usuario.edad }} años</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Usuario',
  props: {
    usuario: {
      type: Object,
      required: true
    }
  }
};
</script>