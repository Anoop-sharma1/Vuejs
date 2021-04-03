<template>
    <div>
        <input type="text" placeholder="Enter Name" name="username" id="" v-model="loginform.username"><br><br>
        <input type="password" placeholder="Enter Password" name="password" id="" v-model="loginform.password"><br><br>
        <button v-on:click="logInData()">Login</button>
    </div>
</template>

<script>
export default {
    name: 'Login',
    methods:{
        logInData() {
            console.log(this.loginform);
        }
    },
    data() {
        return {
            loginform:{
                username:null,
                password:null,
            }
        }
    }
}
</script>