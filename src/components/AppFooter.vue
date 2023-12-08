<script>
import AppMainFooter from './AppMainFooter.vue';
import AppBottomFooter from './AppBottomFooter.vue';

export default {
    name: 'Footer',
    components: {
        AppMainFooter,
        AppBottomFooter,
    }
};
</script>

<template>
    <footer>
        <AppMainFooter />
        <AppBottomFooter />
    </footer>
</template>


<style scoped lang="scss">
footer {
    background-color: #303030;
}
</style>