<template>
    <div class="section">
        <Section01_Main />
    </div>
</template>

<script>
import Section01_Main from '~/components/mocules/section01/Main.vue';

export default {
    components: { Section01_Main },
};
</script>

<style lang="scss" scoped>
.section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    width: 100%;
}
</style>
