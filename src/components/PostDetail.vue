<template>
<div class="post">
    <h3>{{props.title }}</h3> 
    <p>{{ props.content }}</p>
    <button @click="handleClick"></button>    
</div>
</template>

<script lang="ts" setup>
import { defineProps, defineEmits } from 'vue';

   const props = defineProps({
        title: {
            type: String,
             required: true
        },
        content:{
           type: String,
           required: true,
           default: "Este post no tiene contenido"
        }
    })

    const emit = defineEmits(['sayHi'])

        const handleClick = () => {
          emit("sayHi", "hola")
        }

</script>

<style scoped>
.post{
    width: 300px;
    height: 100px;
    background-color: antiquewhite;
    border-radius: 10px;
    margin: 10px;
    padding: 10 px;
    }
</style>