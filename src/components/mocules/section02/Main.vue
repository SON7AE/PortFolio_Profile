<template>
    <div class="main">
        <section02_Card />
        <section02_Card />
        <section02_Card />
        <section02_Card />
    </div>
</template>

<script>
import section02_Card from '~/components/atoms/section02/Card.vue';

export default {
    components: { section02_Card },
};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';

.main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    justify-content: space-around;

    gap: 120px;
}
</style>
