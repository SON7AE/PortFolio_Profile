<template>
    <div class="main">
        <Section02_MainTitle />
    </div>
</template>

<script>
import Section02_MainTitle from '~/components/atoms/section02/MainTitle.vue';

export default {
    components: { Section02_MainTitle },
};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';

.main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
</style>
