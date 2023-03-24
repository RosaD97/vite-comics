<script>
export default {
    name: 'Card',
    props: {
        img: String,
        title: String
    }
}
</script>


<template>
    <div class="cards">
        <div><img :src="img" alt=""></div>
        <span>{{ title }}</span>
    </div>
</template>

<style></style>