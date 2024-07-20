<template>
    <h3>{{ counter }}</h3>
    <button @click="addCounter">Incrementar</button> 
</template>
<script lang="ts">
import { ref} from 'vue';
    let counter = ref(0)
    const addCounter = () => {
        counter.value++
    }
</script>

<style>
h3{
    color: rgb(33, 30, 46);
}
</style>