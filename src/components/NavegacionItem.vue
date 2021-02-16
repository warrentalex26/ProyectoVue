<template>
    <li class="nav-item" v-bind:style="{ backgroundColor:colorRandom, border: '1px solid yellow' }">
              <a class="nav-link" href="#">{{navegacionData.titulo}}</a>
    </li>
</template>

<script>
export default {
    name: "NavegacionItem",
    data() {
    return {
      mostrarActivo: true,
      colorRandom: "#" + Math.floor(Math.random() * 6777215).toString(16), //floor redondea hacia abajo un numero, random nos genera un numero aleatorio y lo multiplicamos por el maximo valor posible, y lo convertimos a cadena de texto con 16 para que devuelva un valor hexadecimal
    };
  },
  props:{
      navegacionData: Object
  }
}
</script>

<style>

</style>