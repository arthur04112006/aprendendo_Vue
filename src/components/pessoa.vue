<template>
    <div>
        <div>
            <h1>descrição da pessoa: {{nome}} </h1>
        <Info/>
        </div>
        
        <div>
            <Form/>
        </div>      
    </div>
</template>
<script>
import Info from './info.vue'
import Form from './form.vue'
export default {
    name: 'Pessoa',
    components: {
        Info, Form
    },
    data(){
        return{
            nome: 'arthur',
        }
    }
}
</script>
