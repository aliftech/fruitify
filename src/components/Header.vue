<template>
    <main>
        <router-link to="/">
            <img alt="Vue logo" src="../assets/logo.png">
        </router-link>
        
        <br>
        <div class="container">
            <div class="alert alert-primary" role="alert"><h1>{{msg}}</h1></div> <br>
        </div>
        <button class="mb-5" v-on:click="$emit('random-fruits')">Random Fruits</button>
    </main>
</template>

<script>
export default {
    data() {
        return {
            msg: 'WELCOME TO FRUITIFY'
        }
    }
}
</script>

<style scoped>
    main {
        text-align:center;
    }

    main button {
        width: 150px;
        height: 45px;
        background-color: slategrey;
        color: white;
        border: none;
    }

    h1 {
        color:slategrey;
    }
</style>