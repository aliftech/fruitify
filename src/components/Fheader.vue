<template>
    <main>
        <router-link to="/">
            <img alt="Vue logo" src="../assets/logo.png">
        </router-link>
        <br>
        <div class="container">
            <div class="alert alert-primary" role="alert"><h1> {{msg}} </h1></div>
        </div>  <br>
    </main>
</template>

<script>
export default {
    data() {
        return {
            msg: 'ABOUT FRUITIFY'
        }
    }
}
</script>

<style scoped>
    main {
        text-align: center;
    }

    h1 {
        color:slategrey;
    }
</style>