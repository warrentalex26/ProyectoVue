<template>
    <div>
        {{mensajes.texto2}}
        <div v-html="mensajes.texto2">
            
        </div>
        <div>
            <!--<h1>{{colores[1]}}</h1>-->
            <ul>
                <li v-for="color in colores" v-bind:key="color">Color: {{color}}</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MiComponente',
    data(){
        return {
            libro: {
                autor: "Alexander Talavera",
                titulo: "Las mil y una noche"
            },
            mensajes:{
                texto1: "Cadena de texto",
                texto2: "<h1>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repudiandae, nisi!</h1> <p>Etiqueta P</p>"
            },
            colores:["Rojo", "Verde", "Amarillo", "Azul"]
        }
    }
}
</script>

<style>

</style>