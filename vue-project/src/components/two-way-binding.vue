<template>
<br/>
<div style="border:solid 1px saddlebrown">
    <h1>Two way data Binding</h1>
    <!-- <input type="text" v-model="count">
    <h2>{{count}}</h2> -->
    <input type="text" placeholder="Enter Email" v-model="email"/><br/><br/>
    <input type="password" placeholder="Enter password" v-model="password"><br/><br/>
    <button v-on:click="getData" type="button">get value</button>
</div>
</template>
<script lang="ts">
export default{
    name:"two-way-binding",

    data(){
        return{
            email:null,
            password:null,
        }
    },
    methods:{
         getData(){
        console.warn(this.email,this.password);
        }
    }
}

</script>