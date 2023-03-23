<script >
export default {
    data(){
        return {
            links: [
                {
                    name: 'CHARACTERS',
                    link: '#'
                },
                {
                    name: 'COMICS',
                    link: '#'
                },
                {
                    name: 'MOVIES',
                    link: '#'
                },
                {
                    name: 'TV',
                    link: '#'
                },
                {
                    name: 'GAMES',
                    link: '#'
                },
                {
                    name: 'COLLECTIBLES',
                    link: '#'
                },
                {
                    name: 'VIDEOS',
                    link: '#'
                },
                {
                    name: 'FANS',
                    link: '#'
                },
                {
                    name: 'NEWS',
                    link: '#'
                },
                {
                    name: 'SHOP',
                    link: '#'
                }
            ]

        }
    },
    components: {
        name: 'Menu'
    }
}
</script>

<template>
    <div>
        <ul>
            <li v-for="item in links"><a :href="item.link">{{ item.name }}</a></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
li {
    list-style: none;
    & a{
        text-decoration: none;
        // padding: 0 20px 0 20px;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        font-size: 13px;
        font-weight: 700;
        color: $third-color;
        padding-bottom: 20px;
        &:hover{
            color: $primary-color;
            border-bottom: 3px solid $primary-color;
        }
    }
}
ul{
    display: flex;
    justify-content: space-between;
}
div{
    width: 44.0625rem;
}
</style>
