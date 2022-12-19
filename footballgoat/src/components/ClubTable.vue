<template>
    <ul class="list-group list-group-flush">
        <li class="list-group-item">{{data.name}}</li>
        <li class="list-group-item">{{data.description}}</li>
    </ul>
</template>

<script>
import axios from 'axios'

export default{
    name: "club-table",
    props: {
        data: Object
    }
}
</script>
