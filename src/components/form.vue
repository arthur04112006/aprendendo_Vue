<template>
  <div>
    <form action="" @submit="captarDadosFormulario($event)">
      <div>
        <input type="text" v-model="name" />
      </div>
      <div>
        <input type="text" v-model="email" />
      </div>
      <div>
        <Submit />
      </div>
    </form>
  </div>
</template>
<script>
import Input from "./form/input.vue";
import Submit from "./form/submit.vue";
export default {
  name: "Form",
  components: {
    Input,
    Submit,
  },
  data() {
    name: ''
    email: ''
  },
  methods: {
    captarDadosFormulario(e) {
        e.preventDefault();

        const name = this.name;
        const email = this.email;

        console.log("o nome e o email são: " + name + " // " + email)
    },
  },
};
</script>