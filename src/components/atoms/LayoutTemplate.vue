<template>
    <div class="layout">
        <slot></slot>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';

.layout {
    width: calc(100% - 48px);
    max-width: 1920px;

    padding: 24px 32px;

    background-color: $color-black;
    border-radius: 5px;
}
</style>
