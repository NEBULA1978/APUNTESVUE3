<!-- doc v-for
(opens new window)
La directiva v-for se usa para iterar sobre una lista de elementos.
Para darle a Vue una pista para que pueda rastrear la identidad de cada nodo y, por lo tanto, reutilizar y reordenar los elementos existentes, debe proporcionar un atributo key único p -->

<script setup>
const name = "Vue 3";
const arrayFrutas = [
    {
        name: "Manzana",
        price: "$1.00",
        description: "Una manzana",
    },
    {
        name: "Pera",
        price: "$2.00",
        description: "Una pera",
    },
    {
        name: "Naranja",
        price: "$3.00",
        description: "Una naranja",
    },
];
</script>

<template>
    <h1>Hola {{ name }}!</h1>
    <ul>
        <li v-for="fruta in arrayFrutas" :key="name">
            {{ fruta.name }} - {{ fruta.price }} - {{ fruta.description }}
        </li>
    </ul>
</template>

