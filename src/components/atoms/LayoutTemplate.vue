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
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    width: calc(100% - 48px);
    max-width: 1920px;

    padding: 24px 32px;
    gap: 120px;

    background-color: $color-black;
    border-radius: 8px;
}
</style>
