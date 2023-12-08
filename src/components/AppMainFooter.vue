<script>
import AppMfLeft from './AppMfLeft.vue';

export default {
    name: 'MainFooter',
    components: {
        AppMfLeft,
    }
};
</script>

<template>
    <div class="main-footer">
        <div class="mf-content">
            <AppMfLeft />
        </div>
    </div>
</template>


<style scoped lang="scss">
.main-footer {
    width: 100%;
    height: 370px;
    background-image: url("/img/footer-bg.jpg");
    background-size: cover;
}

.mf-content {
    width: 80%;
    margin: 0 auto;
}
</style>