<script setup>

import Tarjeta from './components/Tarjeta.vue';
import Producto from './components/Producto.vue';
import Avatar from './components/Avatar.vue';
import Usuario from './components/Usuario.vue';


</script>
<script>


export default {
  components: {
    Usuario
  },
  data() {
    return {
      usuario1: {
        nombre: 'Juan',
        apellido: 'Pérez',
        edad: 30
      }
    };
  }
};
</script>


<template>
<Tarjeta nombre="Chaqueta" descripcion="Esto es una chaqueta." />
<Producto nombre="Laptop" :precio="100000" />
<Avatar url="https://via.placeholder.com/150" :tamaño="100" />
<div class="d-flex flex-wrap">
    <Usuario :usuario="usuario1" />

  </div>

</template>


<style scoped>

</style>
