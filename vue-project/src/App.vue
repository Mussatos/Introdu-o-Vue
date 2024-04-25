<script setup>

import Tabela from './components/Tabela.vue'
import Formulario from './components/Formulario.vue'

const pessoas = [
{
  nome: "Antonio Mussato",
  cpf: "025.022.025-54",
  categoria: "B"
},
{
  nome: "Lian Miranda",
  cpf: "025.022.025-30",
  categoria: "A"
},
{
  nome: "Gabriel Buchara",
  cpf: "025.022.015-30",
  categoria: "C"
}
]
</script>

<template>
    <main>
      <Formulario />
      <Tabela :pessoas="pessoas"/>

    </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
