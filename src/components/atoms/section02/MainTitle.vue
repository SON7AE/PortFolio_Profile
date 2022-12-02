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
        font-family: 'SF Pro Display', sans-serif;
        font-weight: 800;
        font-size: 8em;
    }
    &__subTitle {
        font-family: 'San Francisco';
        font-weight: 500;
        font-size: 1.25em;
    }
}
</style>
