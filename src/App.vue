<template>
  <div id="app">
  <h1>Minha página</h1>
  

  <div v-for="cliente in clientes" :key="cliente.id" >
    <Cliente :cliente="cliente" :show="true" />
  </div>

  </div>
</template>

<script>
import Cliente from './components/Cliente';

export default {
  name: 'App',
  data() {
    return {
      clientes: [
        {
        id: 1,
        nome:"Eduardo",
        email:"kdkla@kldmas.com",
        idade: "20"
      },
      {
        id:2, 
        nome:"Ednaldo Pereira",
        email:"ednaldopereira.chance@yahoo.com",
        idade: "20"
      },
      {
        id:3,
        nome:"Clebre",
        email:"asdasda@kldmas.com",
        idade: "20"
      },
       {
        id:4,
        nome:"Zlebre",
        email:"asdasdsdasda@kldmas.com",
        idade: "25"
      }

      ]
    }
  },
  components: {
    Cliente,
    
  }
}
</script>

<style>
</style>
