<template>
    <div>
        <p v-if="error.length">
            <b>Please Correct the following errors</b>
            <u>
                <li v-for="e in error" v-bind:key='e.id'>
                    {{ e }}
                </li>
            </u>
        </p>
        <form @submit="login">
            <input type="text" placeholder="Enter name" name="" id="" v-model="name"><br><br>
            <input type="password" placeholder="Enter password" name="" id="" v-model="password"><br><br>
    <button>Login</button>
        </form>
    </div>
</template>

<script>
export default {
    name : 'Formvalidation',
    data() {
        return {
            error :[],
            name: null,
            password : null
        }
    },
    methods: {
        login(e) {
            if(this.name && this.password) {
                console.log('No Error');
                return true;
            } else {
                if(!this.name) {
                    this.error.push("User Name Is Req.")
                } 
                if (!this.name) {
                    this.error.push("Password Is Req.")
                }

            }

            console.log('hello' , this.error);
            e.preventDefault();
        }
    }
}
</script>