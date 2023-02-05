<template>
<div id="app">
    <Header/>
    <div class="container">
        <div class="row">
            <div class="col-8">  <LisProduct/></div>
            <div class="col-3"> <MyCart/></div>
        </div>      
       </div>
  </div>
</template>

<script>
import Header from './components/MyHeader.vue'
import LisProduct from './components/LisProduct.vue'
import MyCart from './components/MyCart.vue'

export default {
  name: 'App',
  components:{
    Header,
    LisProduct,
    MyCart,
  }
 
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
