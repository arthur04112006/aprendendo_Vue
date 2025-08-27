<template>
    <div>
        <div>
            <Input/>
        </div>
        <div>
            <Input/>
        </div>
        <div>
            <Submit/>
        </div>
    </div>
</template>
<script>
    import Input from './form/input.vue'
    import Submit from './form/submit.vue'
    export default{
        name: 'Form',
        components: {
            Input, Submit
        }
    }
</script>