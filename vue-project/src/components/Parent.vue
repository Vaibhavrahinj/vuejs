<template>
<h1>child to</h1>
<Child name="Vaibhav Rahinj" :user="user" :getData="getData"></Child>
</template>

<script lang="ts">
import Child from './child.vue';
export default {
    name: "parent",
    component: {
        Child
    },
    data() {
        return {
            user: {name: 'sai', email: 'sai@gmail.com'}
        }
    },

methods: {
    getData() {
        console.log("Parent to child ")
    }
}

}
</script>