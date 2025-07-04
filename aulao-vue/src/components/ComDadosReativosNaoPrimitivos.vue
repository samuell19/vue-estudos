<template>
    <div class="componente">
        <h1>Componente com dados reativos não primitivos</h1>
        <p>Nome: {{ pessoa.nome }} | idade: {{ pessoa.idade }}</p>
        <button @click="fazer_aniversario()">Fazer Aniversario</button>
        <button @click="mudar_nome">Mudar Nome</button>
    </div>
</template>

<script setup>
    import { reactive } from 'vue'
    const pessoa=reactive({nome:"Junior duble", idade:21})

    function fazer_aniversario(){
        pessoa.idade +=1
    }
    
    function mudar_nome(){
        pessoa.nome="estopo"
    }
</script>

<style scoped>
</style>