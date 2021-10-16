<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <employees-component></employees-component>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import EmployeesComponent from './components/EmployeesComponent.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    EmployeesComponent
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
