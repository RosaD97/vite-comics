<script >
export default {
    data(){
        return{
            img: './img/dc-logo.png'
        }
    },
    components: {
        name: 'Logo'
    }
}
</script>

<template>
    <img :src="img" alt="logo">
</template>

<style scoped>
</style>
