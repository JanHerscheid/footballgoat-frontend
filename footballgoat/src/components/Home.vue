<div class="container text-center">
    <div class="row">
        <div class="col-lg">
        1 of 2
        </div>
        <div class="col-lg">
            <div class="row row-cols-1">
                <div class="col">Column1</div>
                <div class="col">Column2</div>
            </div>
        </div>
    </div>
</div>

<script>
import axios from 'axios'

export default{
    name: "home",
    methods:{
    },
    mounted: function(){
        let response = axios.get('https://localhost:7001/api/Player')
        console.log(response)
    }
}
</script>