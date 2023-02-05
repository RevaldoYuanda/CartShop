<template>
  <div class="text-center row">
    <div class="card col-3" style="width: 18rem;" v-for="item in products" :key="item.id">
     <img :src="item.gambar" class="card-img-top" :alt="item.nama"/>
     <div class="card-body">
       <p class="card-title">{{item.nama}}</p>
       <p class="card-text">Rp {{item.harga}}</p>
       <a href="#" @click="addToCart(item)" class="btn btn-primary">Add to Cart</a>
     </div>
   </div>
  </div>
   </template>

   <script>
  
  import products from '../mock/products.json'
  export default{
    name: "ProductList",
    data(){
      return{
        products,
      };
    }
  }
  </script>

  <style>
  .card{
    border: none;
  }
</style>