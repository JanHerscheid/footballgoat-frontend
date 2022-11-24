<template>
  <main>
    <div class="h-100 d-flex align-items-center justify-content-center">
      <div>
        <ul v-for="item in apiData">
          <router-link to="/player">
            <button type="button" class="btn btn-outline-dark">{{ item.name }}</button>  
          </router-link>
        </ul>
      </div>
    </div>
    
  </main>
</template>

<script>
import axios from 'axios';
export default{
  name:'Player',
  data () {
    return {}
  },
  mounted(){
    this.getPlayerStats()
  },
  components: {
  },
  methods:{
      async getPlayerStats(){
          await axios.get(`https://localhost:7001/api/Player`).then((response) => {
              this.apiData = response.data;
          });
          console.log(this.apiData);
      }
  }
}
    
</script>