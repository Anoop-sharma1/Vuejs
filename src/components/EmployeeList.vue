<template>
    <div>
        <h1>Employee List</h1>
    </div>
    <div>
        <table border="1px">
            <tr>
                <td>Name</td>
                <td>Salary</td>
                <td>Age</td>
            </tr>

            <tr v-for="item in list" v-bind:key="item.id">
                <td>{{ item.employee_name}}</td>
                <td>{{ item.employee_salary}}</td>
                <td>{{ item.employee_age}}</td>
            </tr>
        </table>
    </div>
</template>

<script>

const axios = require('axios')
export default {
    name:'EmployeeList',
data(){
return {
    list:undefined
}
},
mounted(){
axios.get("http://dummy.restapiexample.com/api/v1/employees").then((res)=>{
    this.list = res.data.data; 
    console.log(res.data.data);
 })
   }
}
</script>