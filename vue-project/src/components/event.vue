<template>
    <!-- <h1 v-on:mousemove="getmouse('function called')" style="color:red;">This is event page</h1> -->
    
    <br/><button v-on:click="getData()">button1</button>&nbsp;
    <h2>{{count}}</h2>
    <button v-on:dblclick="getData1('button double clicked')">button2</button>
    
</template>
<script lang="ts">
import { jsxClosingElement } from "@babel/types";

    export default{
        name:"Home",
        data(){
            return{
                count:0
            }
        },
        methods:{
            getData()
            {
                this.count=this.count+10
            },
            getData1(a:any){
                alert(a);
    
            },
            // getmouse(s:any){
            //     alert(s);
            // }

        }
    }
</script>