<template>
    <h1>Hola {{ name }}!</h1>
    <h2 v-bind:style="styleColor">Hola {{ name }} desde componente EnlacesAtributos</h2>
    <!-- Forma abreviada v-bind -->
    <!-- <h2 :style="styleColor">Hola {{ name }}</h2> -->
</template>

<script setup>
const name = "Vue 3";
const styleColor = "color: red;";
</script>