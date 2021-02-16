<template>
  <ul class="nav">
    <NavegacionItem v-bind:navegacionData="item" v-for="item in itemsDeNavegacion" :key="item"/>

  </ul>
</template>

<script>
import NavegacionItem from "./NavegacionItem";

export default {
  name: "Navegacion",
  components: {
    NavegacionItem,
  },
  data(){
    return{
      itemsDeNavegacion:[
        {
        titulo:'Inicio',
        url:'/inicio'
        },
        {
        titulo:'Quienes Somos',
        url:'/acercade'
        },
        {
        titulo: 'Tienda',
        url:'/tienda'
        },
        {
        titulo:'Contacto',
        url:'https://www.google.com/'         
        },
        {
        titulo:'Mapa',
        url:'https://www.google.com/'  
      }]
    }
  }
};
</script>

<style>
</style>