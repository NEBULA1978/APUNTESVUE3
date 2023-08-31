<script setup>
const name = "Vue 3 desde v-show";
const active = false;
</script>

<template>
    <h1>Hola {{ name }}!</h1>
    <h2 v-show="active">Estoy en true</h2>
</template>

 <!-- v-show

    La directiva v-show se usa para mostrar o ocultar un elemento de la plantilla.
    v-show solo cambia la propiedad display CSS del elemento.
    En términos generales, v-if tiene costos de alternancia más altos mientras que v-show tiene costos de renderización inicial más altos. Así que prefiera v-show si necesita alternar algo con mucha frecuencia, y prefiera v-if si es poco probable que la condición cambie en el tiempo de ejecución. -->