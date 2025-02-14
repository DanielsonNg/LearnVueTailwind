<script setup>
import { ref } from "vue";
import HelloWorld from "../components/HelloWorld.vue"
let username = ref('')
let password = ref('')
let email = ref('')

function submit(e) {
    e.preventDefault()
    console.log('Username: ' + username.value, 'Password: ' + password.value, 'Email: ' + email.value)
}

</script>

<template>
    <h1>Home Page</h1>
    <!-- <HelloWorld /> -->
    <div class="bg-red-100 w-full h-12">

    </div>
    <div>

    </div>
    <form>
        <input type="text" placeholder="Input" v-model="username">
        <input type="text" placeholder="Input" v-model="password">
        <input type="text" placeholder="Input" v-model="email">
        <button @click="submit">Submit</button>
    </form>
    {{ username }} {{ password }} {{ email }}
</template>