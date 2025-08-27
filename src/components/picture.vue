<template>
  <img :src="Avatar" :alt="Descricao" />
</template>
<script>
export default {
  name: "Picture",
  data() {
    return {
      Avatar: "/img/avatar.png",
      Descricao: "Arthur  Nicolas",
    };
  },
};
</script>