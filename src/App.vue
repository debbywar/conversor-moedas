<template>
  <div id="app">
    <h1 class="text-center">Conversor de Moedas</h1>
    <div class="linha">
    <ConversorMoedas moedaA="USD" moedaB="BRL"/>
    <ConversorMoedas moedaA="BRL" moedaB="USD"/>
    </div>
    <div class="linha">
    <ConversorMoedas moedaA="CAD" moedaB="BRL"/>
    <ConversorMoedas moedaA="BRL" moedaB="CAD"/>
    </div>
    <div class="linha">
    <ConversorMoedas moedaA="EUR" moedaB="BRL"/>
    <ConversorMoedas moedaA="BRL" moedaB="EUR"/>
    </div>
  </div>
</template>

<script>
import ConversorMoedas from "./components/ConversorMoedas.vue"
export default {
  name: 'App',
  components: {
    ConversorMoedas
  }
}
</script>

<style>
#app {
  max-width: 900px;
  margin: auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}

.linha {
  display: flex;
  justify-content: space-around;
  margin-top: 40px;
}

.text-center {
  text-align: center;
}
</style>
