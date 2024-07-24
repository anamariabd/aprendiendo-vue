<template>
   <!-- <p v-bind:class="{ 'danger':hasError }"> 
        El mensaje se ha enviado correctamente.
    </p>--> 
    <p v-bind:style="{ backgroundColor:'#ccc' , color:c }">
        El mensaje se ha enviado correctamente.
    </p>
    <button v-on:click="handleClick()"> Cambiar color </button>
</template>
<script lang="ts">
import {ref, defineComponent} from 'vue'
export default defineComponent({
    name:'ClassBind',
    setup() {
        let c = ref('#fff')
        const handleClick = () => {
            c.value = '#ff0000'
        }
        return{
            c, handleClick
        }
    }
})
</script>

<style>
.danger{ color:green}
</style>