<template>
<v-container >
<div class="row">
      <div class="col-md-4 col-lg4" v-for="(data,index) in projects" :key="index">
        <v-img :src="data.image" class="img-fluid" width="400" height="400">
          </v-img>
         <h3 @click="goTodetail()" >{{data.ProjectTitle}}</h3>

      </div>
    </div>
    </v-container>
</template>

<script>
export default {
  name: 'modules',
  data () {
    return {
      title: 'Modules',
      projects:[
      {
        ProjectTitle:"Graafschades",
        image       : require('../assets/images/Graafschades.jpg'),
        ProjectID:1
      },
      {
        ProjectTitle:"Nachtwacht",
        image       : require('../assets/images/Nachtwacht.jpg'),
        ProjectID:2
      },
      ]
    }
  },
  methods:{
  goTodetail() {
    this.$router.push({name:'details'})
  }
  },
};
</script>

<style scoped>
 
</style>