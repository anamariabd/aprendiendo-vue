<template>
  
  <h1>
     Titulo
    </h1>
  <PostList />
</template>

<script lang="ts">
import PostList from './components/PostList.vue'
export default {
  name: 'App',
  components: {
    PostList
  }
}
</script>

<style>
h1{
  color: green;
}
</style>
