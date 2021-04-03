<template>
<div>
    <h1>Home Component</h1>
    <users/>
    <products/>
    <!-- <h1 v-if="show">For Loop in Vue Js </h1> -->
    <!-- <table>
        <tr>
            <td>Id</td>
            <td>Name</td>
            <td>Email</td>
        </tr>
        <tr v-for="user in users" :key='user.id'>
            <td>{{ user.id }}</td>
            <td>{{ user.name }}</td>
            <td>{{ user.email }}</td>
        </tr>
    </table> -->
    <!-- <button v-on:click="display">Toggle Element</button> -->
    <!-- <h2>{{data}}</h2>
    <h2>{{msg}}</h2> -->
    <!-- <button v-on:mouseover="hello('hello call')">Call Hello Function</button> -->
</div>
    
</template>

<script>
import Users from './Users'
import Products from './Products'
export default {
name : 'Home',
props : {
    data : String,
    msg : String
  },
  components:{
      Users,
      Products
  },
data() {
    return {
        users:[
            {id:1, name:'peter' , email:'ac@'},
            {id:2, name:'pete' , email:'abc@'},
            {id:3, name:'petr' , email:'ab@'},
            {id:4, name:'peer' , email:'bc@'},
        ]
    }
},

};
</script>

<style scoped>
    div{
        background-color:rgb(216, 133, 25);
        height: 500px;
    }
</style>
