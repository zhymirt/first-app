<template>
    <div id='body-container'>
        <h1>Welcome to the HomePage!</h1>
        <div>
            <h2>About Me</h2>
            <p>My name is {{name}}. {{about}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'person',
    props: {
        name: String,
        about: String
    },
    data() {
        return {

        }
    }
}
</script>

<style scoped>
    h2 {
        text-align: left;
    }
    #body-container {
        border-radius: 0.25;
    }
</style>