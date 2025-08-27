<template>
  <h1>
    Segundo componente: o valor vai mudar em 1s → {{ nome }}
  </h1>
</template>

<script>
export default {
  name: 'LifeCycle',
  data() {
    return {
      nome: 'joao',
    }
  },
  created() {
    setTimeout(() => {
      this.nome = 'arthur'
    }, 1000)
  },
  mounted() {
    setTimeout(() => {
      this.nome = 'nicolas'
    }, 2000)
  }
}
</script>
