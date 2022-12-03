<template>
    <div class="card">
        <div class="card__image-box">
            <div class="card__image-box__image"></div>
        </div>
        <div class="card__info-box">
            <span class="card__info-box__title"> Weather Web Application </span>
            <span class="card__info-box__subTitle">
                Open Weather API 데이터와 카카오맵 API 데이터를 기반으로 Vue3와 상태관리 라이브러리인 Pinia를 사용하여 만들어보았습니다. Atomic Design
                구조설계를 진행하였습니다.
            </span>
            <div class="card__info-box__skill-box">
                <img src="~/assets/images/vue.png" alt="" class="card__info-box__skill-box__skill" />
                <img src="~/assets/images/pinia.png" alt="" class="card__info-box__skill-box__skill" />
            </div>
            <v-btn color="primary">
                View Full Here
                <i class="fa-solid fa-computer-mouse" style="margin-left: 8px"></i>
                <v-tooltip activator="parent" location="end" style="font-family: 'Pretendard-Regular'">클릭하면 상세페이지로 넘어갑니다.</v-tooltip>
            </v-btn>
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
    flex-direction: column;
    align-items: center;

    width: 600px;

    gap: 24px;

    &__image-box {
        display: flex;
        align-items: center;
        justify-content: center;

        width: 100%;
        height: 500px;

        padding: 40px 24px;

        background-color: $color-white;
        border-radius: 10px;

        &__image {
            width: 100%;
            height: 100%;

            background-image: url('~/assets/images/image-1.png');
            background-size: cover;
            background-position: center;
        }
    }
    &__info-box {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: center;

        width: 100%;

        gap: 8px;

        &__title {
            font-family: 'Roboto', sans-serif;
            font-weight: 700;
            font-size: 2.5em;
            color: $color-white;
        }
        &__subTitle {
            font-family: 'Pretendard-Regular';
            font-size: 1.25em;
            color: rgba($color-gray, 0.6);

            line-height: 1.3;
        }
        &__skill-box {
            display: flex;
            align-items: center;
            justify-content: flex-start;

            width: 100%;

            gap: 8px;
            margin-bottom: 24px;

            &__skill {
                width: 80px;
            }
        }
    }
}
</style>
