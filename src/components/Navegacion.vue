<template>
  <ul class="nav">
    <NavegacionItem titulo="Inicio" />
    <NavegacionItem titulo="Quienes Somos" />
    <NavegacionItem titulo="Tienda" />
    <NavegacionItem titulo="Contacto" />
  </ul>
</template>

<script>
import NavegacionItem from "./NavegacionItem";

export default {
  name: "Navegacion",
  components: {
    NavegacionItem,
  },
  
};
</script>

<style>
</style>