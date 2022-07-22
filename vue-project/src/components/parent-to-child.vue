<template>
<h1>Send data parent to child</h1>
<Child name="Vaibhav Rahinj" :user="user" :getData="getData"></Child>
</template>

<script lang="ts">
import Child from './child.vue'
export default {
    name: "parentToChildVue",
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
