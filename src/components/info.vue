<template>
  <div>
    <div>
      <!-- Input para digitar a condição -->
      <input v-model="status" placeholder="Digite '1' ou '2'" />
      <!-- Mensagem que aparece só se o usuário digitar "estou trabalhando" -->
      <p v-show="status === '1'">to no trampo</p>
      <p v-show="status === '2'">nao to trampandooo</p>
    </div>
    <div>
      <input v-model="status2" placeholder="Digite '1' ou '2'" />
      <!-- Montando logica usando o if-else do Vue -->
      <p v-if="status2 === '1'">so mostra se entrar no vvvvv----ifffff</p>
      <p v-else-if="status2 === '2'">
        mostra cado nao entre entrar. esta no vvvv----elseeee
      </p>
      <p v-else>mensagem padrao antes de entrar nos if else</p>
    </div>

    <p>Utilizo as tecnologias:</p>
    <ul>
      <li>Python</li>
      <li>Vue</li>
      <li>Java</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Info",
  data() {
    return {
      status: "", // valor inicial do input
      status2: "",
    };
  },
};
</script>
