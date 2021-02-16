<template>
  <div id="app">
        <img alt="Vue logo" src="./assets/logo.png">

    <!--<div v-for="x in 16" v-bind:key="x">/**/</div>-->
    <!--<MiComponente v-for="x in 3" v-bind:key="x"/>-->
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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
