<script setup>
import PrimeiroComponent from './components/PrimeiroComponent.vue';
import ComDados from './components/ComDados.vue';
import ComDadosReativosPrimtiivos from './components/ComDadosReativosPrimtiivos.vue';
import ComDadosReativosNaoPrimitivos from './components/ComDadosReativosNaoPrimitivos.vue';

import axios from 'axios';
import { ref, transformVNodeArgs } from 'vue';
const usuarios= ref()
axios.get('http://localhost:3000/usuarios')
  .then((response) => {
    usuarios.value = response.data
  })
</script>

<template>
  <header>Vue</header>
  <ComDados />
  <PrimeiroComponent />
  <ComDadosReativosPrimtiivos />
  <ComDadosReativosNaoPrimitivos />
  <pre>{{ usuarios }}</pre>
</template>

<style scoped>
</style>