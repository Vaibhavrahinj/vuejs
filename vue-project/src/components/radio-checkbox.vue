<template>
<div style="border:solid 2px slateblue">
<h1>Radio-checkbox values</h1>
<div>
<label for="node">Node</label>
<input type="checkbox" value="node" id="node" v-model="technology">

<label for="php">PHP</label>
<input type="checkbox" value="php" id="php" v-model="technology">

<label for="js">JS</label>
<input type="checkbox" value="js" id="js" v-model="technology">
</div>
<h4>Selected Technology:{{technology}}</h4>
<br><br>
<div>
<label for="student">student</label>
<input type="radio" value="student" id="student" name="profesion" v-model="who">

<label for="developer">Developer</label>
<input type="radio" value="developer" id="developer" name="profesion" v-model="who">
<h4>Selected profesion:{{who}}</h4>

</div>
<h4>if else condition</h4>
<h2 v-if="show">If condition</h2>
<h2 v-else>Else Condition</h2>
<button v-on:click="show=!show">Toggle</button>
</div>
</template>

<script lang="ts">
export default{
    name:"RadioCheckbox",
    data(){
        return{
            show:true
        }
        return {
            technology:[],
            who:null

        }
    }
}

</script>