<template>

    <div class="card">
        <b-card>
            <img :src="image">
            <b-card-text>
                <h3 class="text-center card-header"> {{index+1}} - {{fruits.name}} </h3>
            </b-card-text>

            <b-card-text>
                <p class="mt-5"> {{fruits.taste}} </p>
            </b-card-text>
        </b-card>
    </div>

</template>

<script>
export default {
    computed: {
        image() {
        return require('../assets/img/' + this.fruits.image)
        }
    },
    props: ['fruits', 'index']
}
</script>

<style>

</style>