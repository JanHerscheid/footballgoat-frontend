<template>
    <form @submit.prevent="handleSubmit">
        <div class="Register">
            <input type="text" v-model="username" placeholder="username">
            <input type="password" v-model="password" placeholder="password">
            <button>Register</button>
        </div>
    </form>
</template>

<script>
import axios from 'axios'

export default{
    name: "register-form",
    methods:{
        async handleSubmit(){
            const response = axios.post('https://localhost:7001/api/register', {
                username: this.username,
                password: this.password
            });
            console.log(response);
        }
    }
}
</script>