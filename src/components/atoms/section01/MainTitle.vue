<template>
    <div class="main-title">
        <img class="main-title__image" src="~/assets/images/logo.png" alt="로고 이미지" />
        <span class="main-title__title">MARCO'S DEV</span>
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

    margin-top: 100px;

    &__image {
        width: 200px;
        height: 200px;
    }
    &__title {
        font-family: 'GmarketSansMedium';
        font-weight: 700;
        font-size: 10rem;

        color: $color-white;
    }
}
</style>
