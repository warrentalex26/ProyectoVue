<template>
  <ul class="nav">
            <li class="nav-item">
              <a class="nav-link active" href="#">Active</a>
            </li>
            <li class="nav-item" v-bind:style="{ backgroundColor:colorRandom, border: '1px solid yellow' }">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
            </li>
          </ul>
</template>

<script>
export default {
    name: "Navegacion",
    data(){
        return{
            mostrarActivo: true,
            colorRandom: "#" + Math.floor(Math.random()*6777215).toString(16)//floor redondea hacia abajo un numero, random nos genera un numero aleatorio y lo multiplicamos por el maximo valor posible, y lo convertimos a cadena de texto con 16 para que devuelva un valor hexadecimal
        };
    }
}
</script>

<style>

</style>