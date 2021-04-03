<template>
<div id="app">
  <h1>Api Calling</h1>
  <!-- <div v-if="display">
      <h1>Beforedestroy and destroyed life cycle hooks</h1>
  </div> -->
  <!-- <h1>Beforecreated and created life cycle hooks</h1> -->
  <!-- <h1>Beforemount and mounted life cycle hooks</h1> -->
  <!-- <button v-on:click="toggle()">Toggle</button> -->
</div>
<!-- <h1>Form With Radio Button and Checkbox</h1> -->
<!-- <h1>{{title}}</h1> -->
<!-- <Child v-on:changeTitle="updateTitle($event)"/> -->
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <Home data='Anoop Sharma' msg='hiii'/> -->
  <!-- <ClassBinding/> -->
  <!-- <DataBinding/> -->
  <!-- <Props v-bind:name='users'/> -->
  <!-- <Form /> -->
  <!-- <Login/> -->
  <!-- <Formvalidation/> -->
  <!-- <Filter/> -->
  <!-- <LifeCycle /> -->
  <!-- <Mounted/> -->
  <!-- <Destroy /> -->
  <EmployeeList/>
</template>


<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
// import ClassBinding from './components/ClassBinding'
// import DataBinding from './components/DataBinding'
// import Props from './components/Props'
// import Child from './components/Child'
// import Form from './components/Form'
// import Login from './components/Login'
// import Formvalidation from './components/Formvalidation'
// import Filter from './components/Filter'
// import LifeCycle from './components/LifeCycle'
// import Mounted from './components/Mounted'
// import Destroy from './components/Destroy'
import EmployeeList from './components/EmployeeList'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Home,
    // ClassBinding
    // DataBinding
    // Props
    // Child
    // Form
    // Login
    // Formvalidation
    // Filter
    // LifeCycle
    // Mounted
    // Destroy
    EmployeeList
  },
  data() {
    return {
      display : true
      // name:'Anoop Sharma'
      // users:[
      //   {name:"Yadav"},
      //   {name:"Yada"},
      //   {name:"Yaa"},
      //   {name:"Yad"},
      // ]
      
      // title : "props parent"
    }
    
  },
  methods:{
    // toggle() {
    //   this.display= !this.display 
    // }
      // updateTitle(title) {
      //   this.title=title
      // }
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
