<!-- Eventos

    doc eventos

(opens new window)
Podemos usar la directiva v-on, que normalmente acortamos al símbolo @, para escuchar eventos DOM y ejecutar JavaScript cuando se activan. El uso sería v-on:click="handler" o con el atajo, @click="handler". -->

<script setup>
const name = "Vue 3";

// método handleClick
const handleClick = () => {
    console.log("me diste cick");
};
</script>

<template>
    <h1>Hola {{ name }}!</h1>
    <button v-on:click="handleClick">Click aquí</button>
    <button @click="handleClick">Click aquí</button>
</template>
