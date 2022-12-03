<template>
    <div class="main-title">
        <span class="main-title__miniTitle">Marco & 9Diin's</span>
        <span class="main-title__mainTitle">LATEST PORTFOLIO</span>
        <span class="main-title__subTitle">See my latest creations, Get inspired!</span>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';

.main-title {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    gap: 24px;

    color: $color-white;

    &__miniTitle {
        font-family: 'San Francisco';
        font-weight: 400;
        font-size: 1em;
    }
    &__mainTitle {
        font-family: 'GmarketSansMedium';
        font-weight: 700;
        font-size: 6em;
    }
    &__subTitle {
        font-family: 'San Francisco';
        font-weight: 500;
        font-size: 1.25em;
    }
}
</style>
