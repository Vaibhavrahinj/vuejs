<template>
<div style="border:solid 1px coral ;">
    <h2>Hi this is contact page</h2>
    <h3>Email:{{email}}</h3>
    <h3>Contact:{{contact}}</h3>
    <h3>Name:{{getname("Vaibhav Rahinj")}}</h3>
    <h2>Dob:{{getdata('8/2/2015')}}</h2>
    
</div>
</template>

<script lang="ts">
export default{
    name:"test",
    data(){
        return{
            email:"r@gmail.com",
            contact:9876543210,
           
        }
    },
        methods:{
             getname(name:any){
                return name;
            },
            getdata(v:any){
                return v
            }
        }
    }

</script>