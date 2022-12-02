<template>
    <div class="text-box" :data-theme="theme">
        <span class="text-box__text">{{ title }}</span>
        <span class="text-box__text">{{ subTitle }}</span>
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
        title: {
            type: String,
            required: false,
        },
        subTitle: {
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
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;

    font-family: 'San Francisco';
    font-weight: 500;
    font-size: 16px;

    line-height: 1.4;

    &[data-theme='white'] {
        color: $color-white;
    }
    &[data-theme='gray'] {
        color: rgba($color-gray, 0.5);
    }
}
</style>
