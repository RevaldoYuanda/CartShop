<template>
  <div id="app">
    <Header/>
    <div>
      <LisProduct/>
    </div>
  </div>
</template>

<script>
import Header from './components/MyHeader.vue'
import LisProduct from './components/LisProduct.vue'
export default {
  name: 'App',
  components:{
    Header,
    LisProduct
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
