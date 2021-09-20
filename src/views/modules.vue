<template>
<v-app>
<v-content class="row">
      <div class="col-md-4 col-lg4" v-for="(data,index) in products" :key="index">
        <img :src="data.image" class="img-fluid">
         <h3>{{data.productTitle}}</h3>
      </div>
    </v-content>
    </v-app>
</template>

<script>
export default {
  name: 'modules',
  data () {
    return {
      title: 'Home',
      products:[
      {
        productTitle:"ABCN",
        productId:1
      },
      {
        productTitle:"KARMA",
        productId:2
      },
      {
        productTitle:"Tino",
        productId:3
      },
      {
        productTitle:"EFG",
        productId:4
      },
      {
        productTitle:"MLI",
        productId:5
      },
      {
        productTitle:"Banans",
        productId:6
      }
      ]
    }
  }
}
</script>

<style scoped>
 
</style>