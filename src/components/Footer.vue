<script >
import FooterTop from './FooterTop.vue';
import FooterMid from './FooterMid.vue';
import FooterBottom from './FooterBottom.vue';

export default {
    components: {
        name: 'Footer',
        FooterTop,
        FooterMid,
        FooterBottom
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
    <div>
        <FooterBottom></FooterBottom>
    </div>
</template>

<style scoped></style>
