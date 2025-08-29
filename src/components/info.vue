<template>
  <div>
    <Picture />
    <div>
      <h5>{{email}}</h5>
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
    <button @click="showEmail">{{textoBotao}}</button>
    <h3 v-show="mostrarEmail">meu email é: {{email}}</h3>

    <p>Utilizo as tecnologias:</p>
    <ul>
      <li v-for="(tencologia, index) in tecnologiasConhecidas" v-bind:key="index">{{tencologia}}</li>
      <!-- <li>agora apenas o li com v-for é iterado e repetido. se colocar no ul'pai', ai tudo que tem dentro é iterado e repetido</li> -->
    </ul>
    <ul>
      <li v-for="tencologia in frontEnd" :key="tencologia">{{tencologia.language}}</li>
    </ul>
  </div>
</template>

<script>
import Picture from "./picture.vue";
export default {
  name: "Info",
  data() {
    return {
      status: "", // valor inicial do input
      status2: "",
      mostrarEmail: false,
      textoBotao: 'mostrar email',
      tecnologiasConhecidas: ['Python', 'Vue', 'Java'],
      frontEnd: [
        {id:1 ,language: 'Html',},
        {id:2, language: 'Css'},
        {id:3, language: 'Vue'}
      ]
    }
  },
  props: {
    email: String
  },
  components: {
    Picture,
  },
  methods: {
    showEmail() {
      console.log("o botao ta fungando")
      this.mostrarEmail = !this.mostrarEmail
      if (!this.mostrarEmail) {
        this.textoBotao = 'mostrar email'
      }else{
        this.textoBotao = 'ocultar email'
      }
    }
  },
}
</script>
<style scoped>
  input {
    border-style: solid;
    background-color: #4b9fa5;
    color: rgb(147, 178, 255);
    border-radius: 8px;
  }
  ::placeholder {
    color: black;
  }
button {
  background-color: #ffb700;
  border: 2px solid transparent;
  border-radius: 4px;
  transition: background-color 0.5s, border-color 0.5s; /* propriedades que vão animar */
}

button:hover {
  background-color: #c06a00;  /* cor muda com animação */
  border-color: #624600;   /* borda muda com animação */
  border-style: groove;
  border-radius: 10px;
}

</style>
