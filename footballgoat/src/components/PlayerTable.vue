<template>
    <ul class="list-group list-group-flush">
        <li class="list-group-item"></li>
        <li class="list-group-item"></li>
        <li class="list-group-item"></li>
        <li class="list-group-item"></li>
        <li class="list-group-item"></li>
    </ul>
</template>

<script>
import axios from 'axios'

export default{
    name: "player-table",
    props: {
        data: Object
    }
}
</script>
