<template>
  <div class="container">
    <product-details/>
  </div>
</template>

<script>
import ProductDetails from './components/ProductDetails'

export default {
  name: 'App',
  components: {
    ProductDetails
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
.container{
  display: flex;
  flex-direction: column;
  gap: 32px;
  padding-left: calc(50% - 500px);
  padding-right: calc(50% - 500px);
}
</style>
