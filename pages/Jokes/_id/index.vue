<template>
    <div>
        <p>{{joke}}</p>
        <p>{{$route.params.id}}</p>
    </div>
</template>

<script>
    import axios from "axios";

    export default {
        name: "index",
        data(){
            return {
                joke: {}
            }
        },

        async created() {
            const config = {
                headers: {
                    Accept: 'application/json'
                }
            };

            try {
                const res = await axios.get(`https://icanhazdadjoke.com/j/${this.$route.params.id}`, config)
                this.joke = res.data.joke
            }catch (err) {
                console.log(err)
            }
        },
    }
</script>

<style scoped>

</style>
