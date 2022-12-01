<template>
    <div class="home">
        <LayoutTemplate>
            <Header />
            <Section01 />
        </LayoutTemplate>
    </div>
</template>

<script>
import LayoutTemplate from '~/components/atoms/LayoutTemplate.vue';
import Header from '~/components/mocules/Header.vue';
import Section01 from '~/components/organisms/Section01.vue';

export default {
    components: { LayoutTemplate, Header, Section01 },
};
</script>

<style lang="scss" scoped>
@import '~/assets/styles/main.scss';

.home {
    display: flex;
    align-items: center;
    justify-content: center;

    width: calc(100% - 80px);
    padding: 40px;

    background-color: $color-gray;
}
</style>
