<template>
  <main>
      
    <JumboComp />

    <div class="container">
      <ProductComp v-for="(product, index) in products" :key="index" :card="product" />
      <button class="btn brand">LOAD MORE</button>
    </div>

    <MainOption />
      
  </main>
</template>

<script>
import products from '../assets/data/dc-comics.js'
import JumboComp from './JumboComp.vue';
import ProductComp from './ProductComp.vue';
import MainOption from './MainOption.vue';

export default {
  name: 'MainComp',
  components:{
    JumboComp,
    ProductComp,
    MainOption
  },
  data(){
    return{
      products
    }
  }
}
</script>

<style lang="scss" scoped>

  main{
    .container{
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      padding: 40px 0 20px;
      button{
        font-size: 0.8rem;
        font-weight: 600;
        margin-top: 20px;
        padding: 10px 45px;
      }
    }
  }
</style>