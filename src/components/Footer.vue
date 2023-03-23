<script >
import FooterTop from './FooterTop.vue';
import FooterMid from './FooterMid.vue';

export default {
    components: {
        name: 'Footer',
        FooterTop,
        FooterMid
    }
}
</script>

<template>
    <div>
        <FooterTop></FooterTop>
    </div>
    <div>
        <FooterMid></FooterMid>
    </div>
</template>

<style scoped></style>
