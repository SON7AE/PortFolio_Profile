<template>
    <div class="main">
        <div class="main__title">
            <Section01_MainTitle />
            <Section01_TextBox :text="title" />
            <Section01_TextBox :text="subTitle" :theme="'gray'" />
        </div>
        <div class="main__button-box">
            <Button v-for="button in buttonList" :key="button.label" :button="button" />
        </div>
    </div>
</template>

<script>
import Button from '~/components/atoms/Button.vue';
import Section01_MainTitle from '~/components/atoms/section01/MainTitle.vue';
import Section01_TextBox from '~/components/atoms/section01/TextBox.vue';

export default {
    components: { Section01_MainTitle, Section01_TextBox, Button },
    setup() {
        const title = `안녕하세요, 웹 프론트엔드 개발자(Web Front-End Developer) '박성재'입니다. <br /> 2년차 개발자이며, LG U+ / KT 등 대기업 SI 업무와 크리에이터 관련 커뮤니티 자사서비스 개발 경험이 있습니다.`;
        const subTitle = `Hello, I'm 'SungJae Park', a Web Front-End Developer. <br /> As a 2nd year developer, I have experience in SI work for large corporations such as LG U+ / KT and community own service development related to creators.`;
        const buttonList = [
            {
                icon: 'youtube',
                label: 'YOUTUBE',
            },
            {
                icon: 'notion',
                label: 'NOTION',
            },
            {
                icon: 'tistory',
                label: 'TISTORY',
            },
        ];

        return {
            title,
            subTitle,
            buttonList,
        };
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';
.main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    width: 100%;

    gap: 24px;

    &__title {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;

        width: 100%;

        gap: 24px;
        padding-bottom: 24px;

        border-bottom: 1px solid $color-white;
    }
    &__button-box {
        display: flex;
        align-items: center;
        justify-content: space-between;

        gap: 48px;
    }
}
</style>
