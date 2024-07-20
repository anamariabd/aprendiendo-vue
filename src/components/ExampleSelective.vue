<template>
<h1 v-if="age<18">Eres menor de edad</h1> <!-- Alternativa al if y else es v-show hace un display: none si no cumple el nodo-->
<h1 v-else-if="age>18">Eres mayor de edad</h1> <!-- sino tiene el if no se manda parametro con v-else -->

</template>
<script lang="ts" setup>
let age = 10
</script>
<style>
</style>