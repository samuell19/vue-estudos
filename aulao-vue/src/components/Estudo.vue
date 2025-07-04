<template>

</template>

<script setup>
import { ref } from 'vue';
let id=0

const newTodo=('')
const hidden=(ref=false)
const todos= ref=([
    {id: id++, text:"learn html", done: true},
    {id: id++, text:"learn css", done: true},
    {id: id++, text:"learn python", done: true}
])

</script>

<style scoped>

</style>