<template>
    <div class="h-100 d-flex align-items-center justify-content-center">
        <p class="h3">Spelers</p>
    </div>
    <div class="h-100 d-flex align-items-center justify-content-center">
        <ul class="list-group list-group-flush">
            <li class="list-group-item" v-for="item in items" :key="item.id">{{ item.name }}</li>
        </ul>
    </div>    
</template>

<script>
import axios from 'axios'

export default{
    name: "playerlist",
    data() {
        return {
            items: []
        }
    },
    created() {
        this.fetchPlayers();
    },
    methods:{
        //hiermee vult die de items list die hierboven wordt aangemaakt.
        async fetchPlayers() {
            try {
                const response = await axios.get('https://localhost:7001/api/Player');
                this.items = response.data;
            } catch (error) {
                console.error(error);
            }
        }
    }
}
</script>