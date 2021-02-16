<template>
    <div>
        {{mensajes.texto2}}
        <div v-html="mensajes.texto2">
            
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
                texto2: "<h1>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repudiandae, nisi!</h1> <span>Etiqueta Span</span>"
            }
        }
    }
}
</script>

<style>

</style>