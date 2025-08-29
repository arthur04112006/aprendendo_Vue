<template>
    <nav>
        <ul>
            <li v-for="aba in abasMenu" :key="aba">{{aba}}</li>
        </ul>
    </nav>    
</template>
<script>
export default {
    name: 'Nav',
    data() {
        return {
        abasMenu: ['Sobre', 'Home', 'Github']
        }
    }
}
</script>
<style scoped>
    ul {
        list-style: none;
        display: flex;
        background-color: #999;
        justify-content: center;
        width: 100%;
        
    }
    li {
        margin: 10px, 5px;
        padding: 35px, 15px;
        background-color: #717171;
        color: black;
    }
    #home {
        border: solid, 2px, black;
        border-radius: 8px;
        background-color: goldenrod;
        transition: 0.5s;
        color: black;
    }
    #home:hover{
        color: rgb(32, 32, 32);
        background-color: #7a7a7a;
    }
    
</style>