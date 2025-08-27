<template>
    <div>
        <h1>to comecando a entender essa poha</h1>
        <p>meu nome é {{name}}, tenho {{age}} anos. sou {{profissao}} e moro em {{city}}</p>
    </div>
  
</template>

<script>
export default {
  name: 'quemSou',
  data(){
    return {
        name: 'Arthur Gostosao',
        age: '18',
        city: 'cascavel',
        profissao: 'programador'
    }
  }
}
</script>
