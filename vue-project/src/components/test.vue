<template>
    <div>
        <h1>Hi Hello THis is test page</h1>
       <button v-on:click="test()">Click me</button>
    </div>
</template>
<script lang="ts">
    export default{
        name:"Home",
        methods:{
             test(){
                alert("button clicked");
            }
        }
    }

</script>
<style scoped>
    button{
        color: coral;
    }
</style>