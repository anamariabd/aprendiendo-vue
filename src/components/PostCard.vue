<template>
    <div class="post-card">
        <h3>
            Titulo
        </h3>
        <p> Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolorum, iusto autem nesciunt suscipit necessitatibus similique, nulla porro doloremque modi voluptas velit obcaecati quis deserunt tempore, voluptates ab? Modi, id quam.</p>
        <PostButton/>
    </div>
</template>
<script lang="ts" setup>
import PostButton from './PostButton.vue'
</script>

<style scoped>
.post-card{
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid rgb(0, 0, 0);
}
</style>