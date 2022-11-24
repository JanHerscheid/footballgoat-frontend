<template>
    <register-form/>
</template>

<script>
import RegisterForm from '../components/RegisterForm.vue'

export default{
    name:'Register',
    data(){
        return{
            username:'',
            password:''
        }
    },
    components: {
        RegisterForm
    },
}
</script>
