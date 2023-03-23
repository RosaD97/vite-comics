<script >
export default {
    data() {
        return {
            comics: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],
            shop: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            dc: [
                "Terms Of Use",
                "Privacy Policy (New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshops",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us"
            ],
            sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ]
        }
    },
    components: {
        name: 'FooterMid'
    }
}
</script>

<template>
    <div class="bg">
        <div class="container">
            <div class="section">
                <div class="title">DC COMICS</div>
                <span v-for="item in comics"> <a href="#">{{ item }}</a></span>
            </div>

            <div class="section">
                <div class="title">SHOP</div>
                <span v-for="item in shop"> <a href="#">{{ item }}</a></span>
            </div>

            <div class="section">
                <div class="title">DC</div>
                <span v-for="item in dc"> <a href="#">{{ item }}</a></span>
            </div>

            <div class="section">
                <div class="title">SITES</div>
                <span v-for="item in sites"> <a href="#">{{ item }}</a></span>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use '../styles/general.scss' as *;

.bg {
    background-image: url('./img/footer-bg.jpg');
    height: 370px;
}

.container {
    // background
    background-image: url('./img/dc-logo-bg.png');
    background-repeat: no-repeat;
    height: 370px;
    background-position: 700px;

    width: $bigContainer;
    margin: auto;
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    align-content: baseline;
    font-family: $font;

    & a {
        text-decoration: none;
        color: rgb(148, 147, 147);
        display: flex;
        padding: 2px;

        &:hover {
            color: rgb(207, 207, 207);
        }
    }
}

.section {
    padding: 20px;
}

.title {
    font-size: 20px;
    font-weight: 600;
    color: $secondary-color;
}</style>
