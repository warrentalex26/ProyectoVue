<template>
  <div id="app">
        <div class="container">
          
          <div class="row">
            <Navegacion/>
          </div>
          <div class="row">
            <h1>Mi web</h1>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nesciunt dolores est deserunt. In tenetur voluptates distinctio harum enim quae impedit ea laudantium pariatur asperiores saepe et quod, dolore aliquam minus?</p>

          </div>
        </div>
    <MiComponente/>
  </div>
</template>

<script>
import MiComponente from './components/MiComponente'
import Navegacion from './components/Navegacion.vue'

export default {
  name: 'App',
  components: {
    MiComponente,
    Navegacion
  }
}
</script>

<style>

</style>
