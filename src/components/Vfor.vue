<!-- doc v-for
(opens new window)
La directiva v-for se usa para iterar sobre una lista de elementos.
Para darle a Vue una pista para que pueda rastrear la identidad de cada nodo y, por lo tanto, reutilizar y reordenar los elementos existentes, debe proporcionar un atributo key único p -->

<script setup>
const name = "Vue 3";
const arrayFrutas = ["🍎", "🍌", "🍉", "🍓", "🍒"];
</script>

<template>
    <h1>Hola {{ name }}!</h1>
    <ul>
        <li v-for="(fruta, index) in arrayFrutas" :key="index">
            {{ fruta }}
        </li>
    </ul>
</template>
