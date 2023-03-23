<script>
export default {
    data() {
        return {
            links: [
                {
                    name: 'DIGITAL COMICS',
                    img: './img/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    img: './img/buy-comics-merchandise.png'
                },
                {
                    name: 'SUBSCRIPTION',
                    img: './img/buy-comics-subscriptions.png'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    img: './img/buy-comics-shop-locator.png'
                },
                {
                    name: 'DP POWER VISA',
                    img: './img/buy-dc-power-visa.svg'
                },
            ]
        }
    },
    components: {
        name: 'IconsFooterTop'
    }
}
</script>

<template>
    <div>
        <div class="container">
            <div v-for="item in links">
                <img :src="item.img">
                <span>{{ item.name }}</span>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use '../styles/general.scss' as *;
div{
    background-color: $primary-color;
    height: 9.75rem;
    align-items: center;
    display: flex;
    font-family: $font;
    font-weight: 600;
    &.container{
        display: flex;
        width: $Container;
        margin: auto;
        justify-content: space-between;
        color: $secondary-color;
    }
}
img{
    width: 50px;
    margin-right: 10px;
}
</style>
