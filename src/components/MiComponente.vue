<template>
  <div>
    <!--{{ mensajes.texto2 }}-->
    <!--<div v-html="mensajes.texto2"></div>-->

    <div>
      <!--<h1>{{colores[1]}}</h1>-->

      <!--<ul>
        <li v-for="color in colores" v-bind:key="color">Color: {{ color }}</li>
      </ul>-->

      <!--div v-for="color in colores2" v-bind:key="color">
        {{color.nombre}} -
        {{color.nombreIngles}}
        <p>--------------------------</p>
    </div>-->
      <!--<button>Selección</button>-->

      <!--
      Se puede evaluar tambien asi v-if="mostrarBoton == 'xxx'" lo que este entre las comillas
    -->
      <p>{{ mostrarBoton }}</p>

      <div v-if="mostrarBoton == 'clave'">
        Usuario autenticado <button>Boton secreto</button>
      </div>

      <div v-else-if="mostrarBoton">Valor encontrado pero incorrecto</div>

      <div v-else>Valor no encontrado, ingrese un valor</div>

    </div>
  </div>
</template>

<script>
export default {
  name: "MiComponente",
  data() {
    return {
      libro: {
        autor: "Alexander Talavera",
        titulo: "Las mil y una noche",
      },
      mensajes: {
        texto1: "Cadena de texto",
        texto2:
          "<h1>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repudiandae, nisi!</h1> <p>Etiqueta P</p>",
      },
      colores: ["Rojo", "Verde", "Amarillo", "Azul"],
      colores2: [
        {
          nombre: "Rojo",
          nombreIngles: "red",
        },
        {
          nombre: "Verde",
          nombreIngles: "green",
        },
        {
          nombre: "Amarillo",
          nombreIngles: "Yellow",
        },
        {
          nombre: "Morado",
          nombreIngles: "purple",
        },
      ],
      mostrarBoton: "clave",
    };
  },
};
</script>

<style>
button {
  background-color: green;
  padding: 5px 10px;
  color: white;
  border: none;
  border-radius: 100px;
  margin-top: 15px;
  display: inline-block;
}

button:active {
  background: black;
}
</style>