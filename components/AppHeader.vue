<template>
    <header class="header">
        <h1>Dad title</h1>
        <ul>
            <li>
                <nuxt-link to="/">Home</nuxt-link>
                <nuxt-link to="/jokes">Jokes</nuxt-link>
                <nuxt-link to="/about">About</nuxt-link>
            </li>
        </ul>
    </header>
</template>

<script>
    export default {
        name: "AppHeader"
    }
</script>

<style scoped>

</style>
