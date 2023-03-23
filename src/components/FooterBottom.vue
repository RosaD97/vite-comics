<script >
export default {
    components: {
        name: 'FooterBottom'
    }
}
</script>

<template>
    <div class="bigContainer">
        <div class="container">
            <div>
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="socialLink">
                <h3>FOLLOW US</h3>
                <span> <img src="public\img\footer-facebook.png" alt="facebook"></span>
                <span> <img src="public\img\footer-twitter.png" alt="twitter"></span>
                <span> <img src="public\img\footer-youtube.png" alt="youtube"></span>
                <span> <img src="public\img\footer-pinterest.png" alt="pinterest"></span>
                <span> <img src="public\img\footer-periscope.png" alt="periscope"></span>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;
@use '../styles/general.scss' as *;

.bigContainer {
    background-color: $fourth-color;
    height: 112px;
    display: flex;
}

.container {
    width: $Container;
    margin: auto;
    display: flex;
    justify-content: space-between;
}

button{
    padding: 10px;
    font-size: 15px;
    background-color: $fourth-color;
    color: $secondary-color;
    border-color: $primary-color;
}
.socialLink{
    display: flex;
    align-items: center;
    & span{
        padding-left: 20px;
    }
    & h3{
        font-family: $font;
        color: $primary-color;
    }
}
</style>
