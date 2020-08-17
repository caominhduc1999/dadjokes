<template>
    <div>
        <nuxt-link :to="'jokes/' + id">
            <p>{{joke}}</p>
        </nuxt-link>
    </div>
</template>

<script>
    export default {
        name: "Joke",
        props: [
            'joke',
            'id'
        ]
    }
</script>

<style scoped>

</style>
