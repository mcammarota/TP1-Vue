<template>
  <div id="app">
    <Tarefa />
  </div>
</template>

<script>
import Tarefa from './components/Tarefa.vue'

export default {
  name: 'App',
  components: {
    Tarefa
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
