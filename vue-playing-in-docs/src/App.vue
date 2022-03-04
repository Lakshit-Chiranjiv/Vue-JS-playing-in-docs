<template>
  <h1>VUE JS - playing in the docs</h1>
  <img alt="Vue logo" src="./assets/logo.png">
  <hr>
  <HelloWorld/>
  <hr>
  <Templates/>
  <hr>
  <Directives/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Templates from './components/Templates.vue'
import Directives from './components/Directives.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Templates,
    Directives
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
