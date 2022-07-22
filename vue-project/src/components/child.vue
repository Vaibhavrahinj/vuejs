<template>
<h2>child data</h2>
        <h2>{{name}}</h2>
         <h2>{{user.name}}</h2>
        <button v-on:click="getData()">call function</button>
</template>

<script lang="ts">
export default{
    name:"Child",
    props: {
        name:String,
        user:Object,
        getData:Function
    }
}
</script>