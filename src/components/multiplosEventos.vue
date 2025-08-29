<template>
  <div>
    <button @click="primeiro($event), segundo($event), terceiro($event)">Ativar MultiplosEventos</button>
    <h4>{{ multiplos_eventos }}</h4>
  </div>
</template>
<script>
export default {
  name: "MultiplosEventos",
  data() {
    return {
        multiplos_eventos: "",
        txt1: "primeiro evento de click",
        txt2: "segundo evendo de click",
        txt3: "terceiro evento de click"
    }
  },
  methods: {
    primeiro(e) {
      this.multiplos_eventos = this.txt1;
    },
    segundo(e) {
      setTimeout(() => this.multiplos_eventos = this.txt2, 1500)
    },
    terceiro(e) {
        setTimeout(() => this.multiplos_eventos = this.txt3, 3000)
      
    },
  },
};
</script>