<template>
    <div>
        <h1>Dadjokes</h1>
        <p>Hello</p>
    </div>
</template>

<script>
    export default {
        name: "about",
        head(){
            return {
                title: 'About the app',
                meta: [
                    {
                        hid: 'description',
                        name: 'description',
                        content: 'this is description',
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>
