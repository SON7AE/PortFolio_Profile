<template>
    <div class="text-box">
        <span v-html="text" :data-theme="theme" class="text-box__text"></span>
    </div>
</template>

<script>
export default {
    props: {
        theme: {
            /**@type {import("vue").ProtoType<Theme>} */
            type: String,
            required: false,
            /**@type {Theme} */
            default: 'white',
        },
        text: {
            type: String,
            required: false,
        },
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';

.text-box {
    display: flex;
    align-items: flex-start;
    justify-content: center;

    &__text {
        font-family: 'Pretendard-Regular';
        font-size: 20px;

        color: $color-white;
        text-align: center;
        line-height: 1.4;

        &[data-theme='gray'] {
            color: rgba($color-gray, 0.5);
        }
    }
}
</style>
