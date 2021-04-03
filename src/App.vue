<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <Home data='Anoop Sharma' msg='hiii'/> -->
  <!-- <ClassBinding/> -->
  <DataBinding/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
// import ClassBinding from './components/ClassBinding'
import DataBinding from './components/DataBinding'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Home,
    // ClassBinding
    DataBinding
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
