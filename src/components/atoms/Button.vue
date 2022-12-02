<template>
    <button @click="moveToLink" class="button">
        <!-- <img :src="`/assets/images/${button.icon}.png`" alt="이력서 이미지" class="button__image" /> -->
        <div class="button__image" :data-theme="button.icon"></div>
        <span class="button__label">{{ button.label }}</span>
    </button>
</template>

<script>
export default {
    props: {
        button: {
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
        background-size: contain;

        &[data-theme='youtube'] {
            background-image: url('~/assets/images/youtube.png');
        }
        &[data-theme='notion'] {
            background-image: url('~/assets/images/notion.png');
        }
        &[data-theme='tistory'] {
            background-image: url('~/assets/images/tistory.png');
        }
    }
    &__label {
        font-family: 'Montserrat', sans-serif;
        font-size: 50px;
        font-weight: 600;

        color: $color-white;
    }
}
</style>
