<script >
import SeriesList from './SeriesList.vue';

export default {
    components: {
        name: 'Main',
        SeriesList
    }
}
</script>

<template>
    <div>
        <div class="jumbotron"></div>
        <div class="container">
            <SeriesList></SeriesList>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use '../styles/general.scss' as *;

div {
    background-color: $third-color;
}

.container {
    width: $Container;
    margin: auto;
    display: flex;
    align-items: center;
    padding: 1.875rem 0 2.5rem 0;

    & h2 {
        color: $secondary-color;
        font-family: $font;
    }
}

.jumbotron {
    height: 25rem;
    background-image: url(../../public/img/jumbotron.jpg);
}
</style>
