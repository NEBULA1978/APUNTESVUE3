 <!-- v-for v-if

    doc v-for v-if

(opens new window)
Cuando existen en el mismo nodo, v-if tiene una prioridad más alta que v-for.
Eso significa que la condición v-if no tendrá acceso a las variables del alcance de v-for: -->

<script setup>
const name = "Vue 3";
const arrayFrutas = [
    {
        name: "Manzana",
        price: "$1.00",
        description: "Una manzana",
        stock: 0,
    },
    {
        name: "Pera",
        price: "$2.00",
        description: "Una pera",
        stock: 10,
    },
    {
        name: "Naranja",
        price: "$3.00",
        description: "Una naranja",
        stock: 20,
    },
];
</script>

<template>
    <h1>Hola {{ name }}!</h1>
    <ul>
        <li v-for="fruta in arrayFrutas" :key="fruta.name" v-if="fruta.stock > 0">
            {{ fruta }}
        </li>
    </ul>

    <ul>
        <template v-for="fruta in arrayFrutas" :key="fruta.name">
            <li v-if="fruta.stock > 0">
                {{ fruta }}
            </li>
        </template>
    </ul>
</template>
