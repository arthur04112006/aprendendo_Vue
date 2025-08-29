<template>
  <div>
    <Nav/>
    <quemSou/>
    <LifeCycle/>
    <Pessoa/>
  </div>
</template>

<script>
import quemSou from './components/quemSou.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/pessoa.vue'
import Nav from './components/nav.vue'

export default{
  components: { quemSou, LifeCycle, Pessoa, Nav },
  name: 'App'
}
</script>
<style>
body {
  background-color : rgba(121, 135, 205, 0.533);
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  color: rgb(56, 55, 55);
  border: 3px;
  display: flex;
  align-content: center;
}
a {
  color: greenyellow;
  border-radius: 6px;
}
  
</style>


