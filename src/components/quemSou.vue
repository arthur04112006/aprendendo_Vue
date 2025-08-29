<template>
  <div>
    <MultiplosEventos />
    <Reutilizacao />
    <h1>to comecando a entender essa poha</h1>
    <p>
      meu nome é {{ name }}, tenho {{ age }} anos. sou {{ profissao }} e moro em
      {{ city }}
    </p>
    <h3>meu github é: <a :href="github" target="blank">Meus Projetos</a></h3>
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
  </div>
</template>

<script>
import MultiplosEventos from "./multiplosEventos.vue";
import Reutilizacao from "./reutilizacao.vue";
export default {
  name: "quemSou",
  data() {
    return {
      name: "Arthur Gostosao",
      age: "18",
      city: "cascavel",
      profissao: "programador",
      github: "https://github.com/arthur04112006",
    };
  },
  components: {
    MultiplosEventos,
    Reutilizacao,
  },
};
</script>
