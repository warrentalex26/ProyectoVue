<template>
  <div id="app">
        <div class="container">
          
          <div class="row">
            <ul class="nav">
            <li class="nav-item">
              <a class="nav-link active" href="#">Active</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
            </li>
          </ul>
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

export default {
  name: 'App',
  components: {
    MiComponente
  }
}
</script>

<style>

</style>
