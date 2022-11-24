<template>
    <login-form/>
</template>

<script>
import LoginForm from '../components/LoginForm.vue'

export default{
    name:'Login',
    data(){
        return{
            username:'',
            password:''
        }
    },
    components: {
        LoginForm
    },
}
</script>
