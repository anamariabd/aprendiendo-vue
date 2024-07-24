<template>
    <div>
        <PostDetail v-for="elem in info" v-bind:key="elem.title"
        :title="elem.title" :content="elem.content" @sayHi="showAlert" />
    </div>
</template>

<script lang="ts" setup>
import PostDetail from './PostDetail.vue'

let info = [{
     title: "Titulo de post 1",
     content: "Lorem ipsum"
    }, {
     title: "Titulo de post 2",
     content: "Lorem ipsum"
    }, {
     title: "Titulo de post 3",
     content: "Lorem ipsum"
    }]

    let emit = ["sayHi"]

    function showAlert(msg:string){
        alert(msg)
    }

</script>
<style scoped>
.container{
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-around;
}
</style>