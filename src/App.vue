<template>
  <div id="app">
    <h1>Minha primeira aplicação utilizando Vue.JS</h1>
    <div class="row">
      <Converter moeda-a="USD" moeda-b="BRL"/>
      <Converter moeda-a="BRL" moeda-b="USD"/>
    </div>
    <div class="row">
      <Converter moeda-a="CAD" moeda-b="BRL"/>
      <Converter moeda-a="BRL" moeda-b="CAD"/>
    </div>
    <div class="row">
      <Converter moeda-a="EUR" moeda-b="BRL"/>
      <Converter moeda-a="BRL" moeda-b="EUR"/>
    </div>
  </div>
</template>

<script>

import Converter from './components/Converter.vue';

export default {
  name: 'app',
  components: {
    Converter
  }
}
</script>

<style>

#app {
  margin: 0 auto;
  max-width: 900px;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;  
  color: #2c3e50;
  margin-top: 60px;
}

.row {
  display: flex;
  justify-content: space-around;
}

h1 {
  text-align: center;
}

</style>
