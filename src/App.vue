<template>
  
  <h1>
     Titulo
    </h1>
  <ClassBind />
</template>

<script lang="ts">
import PostContainer from './components/PostContainer.vue';
import CounterOption from './components/CounterOption.vue'
//import CounterComposition from './components/CounterComposition.vue'
import ExampleFor from './components/ExampleFor.vue'
import ClassBind from './components/ClassBind.vue'
export default {
  name: 'App',
  components: {
    ClassBind
  }
}
</script>

<style>
h1{
  color: green;
}
</style>
