<template>
  <div>
    <quemSou/>
    <LifeCycle/>
    <Pessoa/>
  </div>
</template>

<script>
import quemSou from './components/quemSou.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/pessoa.vue'

export default{
  components: { quemSou, LifeCycle, Pessoa },
  name: 'App'
}
</script>


