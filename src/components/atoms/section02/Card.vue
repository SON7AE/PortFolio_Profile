<template>
    <div class="card">
        <div class="card__thumbnail"></div>
        <div class="card__info-box">
            <div class="card__info-box__header">
                <span class="card__info-box__header__date">Dec 1, 2022</span>
                <span class="card__info-box__header__label">Completed</span>
            </div>
            <div class="card__info-box__work">
                <span class="card__info-box__work__name">OpenWeather API를 활용한 날씨 웹 애플리케이션</span>
            </div>
            <div class="card__info-box__language"></div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';

.card {
    display: flex;

    width: 640px; // 수정
    height: 280px;

    padding: 40px;
    gap: 24px;

    cursor: pointer;

    &:hover {
        border-radius: 5px;
        background-color: rgba($color-gray, 0.2);
        transition: 1s ease;
    }

    &__thumbnail {
        width: 280px;

        border-radius: 5px;

        background-image: url('~/assets/images/image-1.png');
        background-position: center;
        background-size: cover;
    }
    &__info-box {
        display: flex;
        flex-direction: column;
        align-items: flex-start;

        width: calc(100% - 256px);

        gap: 24px; // 수정

        &__header {
            display: flex;
            align-items: center;
            justify-content: space-between;

            width: 100%;

            font-family: 'San Francisco';
            font-size: 1em;
            color: $color-white;

            &__date {
            }
            &__label {
                padding: 4px;

                border: 1px solid $color-green;
                border-radius: 5px;
            }
        }
        &__work {
            width: 100%;

            &__name {
                font-family: 'Pretendard-Regular';
                font-size: 1.5em;
                color: $color-white;
            }
        }
    }
}
</style>
