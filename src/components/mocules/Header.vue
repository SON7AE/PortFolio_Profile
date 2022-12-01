<template>
    <header class="header">
        <div class="header__box">
            <HeaderTextBox :title="title" :sub-title="subTitle" :theme="'white'" />
            <HeaderTextBox :title="'Park'" :sub-title="'SungJae'" :theme="'gray'" />
        </div>
        <HeaderTextBox :title="'Marco'" :sub-title="'9Diin'" :theme="'white'" />
    </header>
</template>

<script>
import HeaderTextBox from '~/components/atoms/HeaderTextBox.vue';

export default {
    components: { HeaderTextBox },
    setup() {
        const title = 'Front End Developer';
        const subTitle = '& Degital Creator';

        return {
            title,
            subTitle,
        };
    },
};
</script>

<style lang="scss" scoped>
.header {
    display: flex;
    align-items: center;
    justify-content: space-between;

    width: 100%;
    padding-bottom: 16px;

    border-bottom: solid 1px white;

    &__box {
        display: flex;
        align-items: center;
        justify-content: flex-start;

        gap: 160px;
    }
}
</style>
