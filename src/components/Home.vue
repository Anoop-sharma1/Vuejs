<template>
<div>
    <h1 style="    background: yellow;">Home Component</h1>
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
export default {
name : 'Home',
props : {
    data : String,
    msg : String
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
