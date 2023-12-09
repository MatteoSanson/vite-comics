<script>
import AppButtonLeft from './FooterBottom/AppButtonLeft.vue';
import AppBtmRight from './FooterBottom/AppBtmRight.vue';

export default {
    name: 'BottomFooter',
    components: {
        AppButtonLeft,
        AppBtmRight
    }
};
</script>

<template>
    <div class="btm-footer">
        <div class="btm-left">
            <AppButtonLeft />
        </div>

        <div class="btm-right">
            <AppBtmRight />
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;

.btm-footer {
    width: 80%;
    height: 110px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

}
</style>