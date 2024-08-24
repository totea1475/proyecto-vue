<!-- eslint-disable vue/multi-word-component-names -->

<template>
    <h1>Hola Mundo</h1>
    <p>{{ contadores }}</p>
    <button @click="incrementar">Incrementar</button>
    <button @click="decrementar">Decrementar</button>
    </template>

    <script setup>
    import {ref} from 'vue';
    const contadores = ref(0);
    const incrementar = () =>{
        contadores.value++;
    }
    const decrementar = () =>{
        contadores.value--;
    }
</script>
    
    
    <style scoped>
    p{
      color: red;
    }
    </style>