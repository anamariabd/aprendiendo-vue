<template><ul>
    <li v-for="country in countries" v-bind:key="country.code"> {{ country.name }}  </li>
</ul>
</template>
<script lang="ts" setup>
import {Ref, ref} from 'vue';
/*let countries:Ref<Array<string>> = ref([
    'Spain', 'France', 'UK', 'Italy', 'Portugal'
])*/
interface Country {code: string, name: string}
let countries:Ref<Country<>> = ref([
{code: 'es', name: 'Spain'},{code: 'fr', name: 'France'},{code: 'en', name: 'UK'},{code: 'es', name: 'Italy'}
])
</script>
<style>
</style>