<template>
    <form @submit.prevent="handleSubmit">
        <div class="Login">
            <input type="text" v-model="username" placeholder="username">
            <input type="password" v-model="password" placeholder="password">
            <button>Login</button>
        </div>
    </form>
</template>

<script>
import axios from 'axios'

export default{
    name: "login-form",
    methods:{
        async handleSubmit(){
            const response = axios.post('', {
                username: this.username,
                password: this.password
            });
            console.log(response);
        }
    }
}
</script>
