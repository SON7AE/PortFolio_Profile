<template>
    <button @click="moveToLink" class="button">
        <img :src="`src/assets/images/${resume.icon}.png`" alt="이력서 이미지" class="button__image" />
        <span class="button__label">{{ resume.label }}</span>
    </button>
</template>

<script>
export default {
    props: {
        resume: {
            type: Object,
            required: false,
        },
    },
    setup() {
        const moveToLink = () => {
            console.log('버튼이 클릭되었습니다.');
        };

        return {
            moveToLink,
        };
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';

.button {
    display: flex;
    align-items: center;
    justify-content: center;

    height: 64px;

    gap: 12px;
    padding: 40px 24px;

    outline: none;
    border: 1px solid $color-white;
    border-radius: 35px;
    background: transparent;

    cursor: pointer;

    &__image {
        width: 50px;
        height: 50px;
    }
    &__label {
        font-family: 'Montserrat', sans-serif;
        font-size: 50px;
        font-weight: 600;

        color: $color-white;
    }
}
</style>
