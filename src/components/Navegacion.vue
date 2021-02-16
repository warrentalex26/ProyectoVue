<template>
  <ul class="nav">
    <NavegacionItem v-bind:navegacionData=" {titulo:'Inicio', url:'https://www.google.com/'}"/>
    <NavegacionItem v-bind:navegacionData=" {titulo:'Quienes Somos', url:'https://www.google.com/'} "/>
    <NavegacionItem v-bind:navegacionData=" {titulo:'Tienda', url:'https://www.google.com/'} "/>
    <NavegacionItem v-bind:navegacionData=" {titulo:'Contacto', url:'https://www.google.com/'} "/>
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