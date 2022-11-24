<template>

</template>

<script>
import axios from 'axios'
import { onMounted } from 'vue';

export default{
    name: "playerlist",
    methods:{
    },
    mounted: function(){
        let response = axios.get('https://localhost:7001/api/Player')
        console.log(response)
    }
}
</script>