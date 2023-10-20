<template>
   <v-container>
    <div class="furniturecard">
        
                   <FurnitureCard v-for="product in products" :key="product.id" >
                    <template v-slot:title>{{product.title}}</template>
                    <template v-slot:subtitle>{{product.price}}</template>
                    </FurnitureCard>
    </div>
    
   </v-container>
  </template>

  <script >
  import FurnitureCard from '../components/FurnitureCard.vue'
 export default {
    components:{ FurnitureCard  },
  data() {
    return {
        products: []  

    }
  },
  methods: {
    getProducts() {
      fetch('file.json')
        .then(response => response.json())
        .then(data=> this.products = data.filter(t => t.id ))
    }
  }
  , 
  mounted(){
    this.getProducts()
  }
}
  </script>
