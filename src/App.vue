
/* Create un nuovo progetto utilizzando Vue CLI e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone. */
<template>
  <div id="app">
    
    <HeaderComp />
    <MainComp />
    <FooterComp />

  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp
  }
}
</script>

<style lang="scss">
//general
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

</style>
