<script >
export default {
    components: {
        name: 'Main'
    }
}
</script>

<template>
    <div>
        <div class="container">
            <h2>-Content goes here-</h2>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use '../styles/general.scss' as *;

div{
    height: 8.25rem;
    background-color: $third-color;
}
.container{
    width: $bigContainer;
    margin: auto;
    display: flex;
    align-items: center;
    & h2{
        color: $secondary-color;
        font-family: $font;
    }
}
</style>
