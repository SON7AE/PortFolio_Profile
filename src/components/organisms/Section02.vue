<template>
    <div class="section">
        <Section02_Header />
        <Section02_Main />
    </div>
</template>

<script>
import Section02_Header from '~/components/mocules/section02/Header.vue';
import Section02_Main from '~/components/mocules/section02/Main.vue';

export default {
    components: { Section02_Header, Section02_Main },
};
</script>

<style lang="scss" scoped>
.section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    width: 100%;

    gap: 80px;
}
</style>
