<template>
    <div>
        <h1>
            componente com dados
        </h1>
        <p>
            Nome: {{nomeProduto}} - {{ codigoProduto }} 
        </p>
    </div>

</template>
<style scoped>
</style>
<script setup>
const nomeProduto="lapiseira"
const codigoProduto="#6969"
</script>



<style scoped>
div{
    text-align: center;
    border:2px solid rgb(10,69,4);
    background-color:#050d04;
    border-radius: 15px;
    margin: 30px;
    padding: 10px;
}

p{
    font-size: 1.5rem;
}
</style>