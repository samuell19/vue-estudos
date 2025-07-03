<template>
    <div class="componente">
        <h1>Componente com dados reativos</h1>
        <p>Nome: {{ nome }} | idade: {{ idade }}</p>
        <button @click="fazer_aniversario">Fazer Aniversario</button>
        <button @click="mudar_nome">Mudar Nome</button>
    </div>
</template>

<script setup>
    import { ref } from 'vue'
    const nome=ref("capixaba")
    const idade=ref("789")

    function fazer_aniversario(){
        idade.value +=1
    }
    
    function mudar_nome(){
        nome.value="estopo"
    }
</script>

<style scoped>
</style>