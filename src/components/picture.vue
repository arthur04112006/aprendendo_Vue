<template>
  <img :src="Avatar" :alt="Descricao"/>
  <MudarImagem @mudarImagem="trocarImagem"/>
</template>
<script>
import MudarImagem from './mudarImagem.vue';
export default {
  name: "Picture",
  data() {
    return {
      Avatar: "/img/avatar.png",
      Descricao: "Arthur  Nicolas",
    };
  },
  components: {
    MudarImagem
  },
  methods: {
    trocarImagem() {
      this.Avatar = '/img/avatar2.png'
    }
  }
};
</script>