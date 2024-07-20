<template>
  
  <h1>
     Titulo
    </h1>
  <CounterComposition />
</template>

<script lang="ts">
import PostContainer from './components/PostContainer.vue';
import CounterOption from './components/CounterOption.vue'
import CounterComposition from './components/CounterComposition.vue'

export default {
  name: 'App',
  components: {
    CounterComposition
  }
}
</script>

<style>
h1{
  color: green;
}
</style>
