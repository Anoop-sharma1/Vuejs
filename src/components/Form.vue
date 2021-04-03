<template>
    <div>
        <input type="text" placeholder="Enter Name" v-model="signup.username"><br><br><br>
        <input type="password" placeholder="Enter password" v-model="signup.password"><br><br><br>
        <input type="checkbox" id="cricket" value="cricket" v-model="signup.hobbies">
        <label for="cricket" >
            Cricket
        </label>
        <input type="checkbox" id="football" value="football" v-model="signup.hobbies">
        <label for="football" >
            Football
        </label>

        <input type="radio" id="male" value="male" v-model="signup.gender">
        <label for="male" >
            Male
        </label>
        <input type="radio" id="female" value="female" v-model="signup.gender">
        <label for="female" >
            Female
        </label>
        <button v-on:click="signUpUser()">Sign Up</button>
    </div>
</template>

<script>
export default {
    name:'Form',
    data() {
       return {
           signup:{
            username : null,
            password : null,
            hobbies : [],
            gender : null
        }
       }
    },
    methods:{
        signUpUser() {
            console.log(this.signup);
        }
    }
}
</script>