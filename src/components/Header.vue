<script >
import Logo from './Logo.vue';
import Menu from './Menu.vue';

export default {
    components: {
        name: 'Header',
        Logo,
        Menu
    }
}
</script>

<template>
    <div class="container">
        <div>
            <Logo></Logo>
        </div>
        <div class="menu">
            <Menu></Menu>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use '../styles/general.scss' as *;


div.container {
    height: 7.25rem;
    display: flex;
    justify-content: space-between;
    width: $bigContainer;
    margin: auto;
    margin-top: .9375rem;
}
.menu{
    vertical-align: bottom;
}
</style>
