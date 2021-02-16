<template>
  <div id="app">
        <div class="container">
          
          <div class="row">
            <Navegacion/>
          </div>
          <div class="row">
            <Contenido/>
          </div>
        </div>
    <!--<MiComponente/>-->
  </div>
</template>

<script>
//import MiComponente from './components/MiComponente'
import Navegacion from './components/Navegacion.vue'
import Contenido from './components/Contenido.vue'

export default {
  name: 'App',
  components: {
    //MiComponente,
    Navegacion,
    Contenido
  }
}
</script>

<style>

</style>
