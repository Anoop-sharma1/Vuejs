<template>
<h1>{{title}}</h1>

<Child v-on:changeTitle="updateTitle($event)"/>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <Home data='Anoop Sharma' msg='hiii'/> -->
  <!-- <ClassBinding/> -->
  <!-- <DataBinding/> -->
  <!-- <Props v-bind:name='users'/> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
// import ClassBinding from './components/ClassBinding'
// import DataBinding from './components/DataBinding'
// import Props from './components/Props'
import Child from './components/Child'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Home,
    // ClassBinding
    // DataBinding
    // Props
    Child
  },
  data() {
    return {
      // users:[
      //   {name:"Yadav"},
      //   {name:"Yada"},
      //   {name:"Yaa"},
      //   {name:"Yad"},
      // ]
      
      title : "props parent"
    }
    
  },
  methods:{
      updateTitle(title) {
        this.title=title
      }
    }
};
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
