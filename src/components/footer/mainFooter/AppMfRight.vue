<script>
export default {
    name: 'MainRightFooter',
    data() {
        return {}
    }
};
</script>

<template>
    <div class="img-bg-foot">
        <img src="/img/dc-logo-bg.png" alt="dc logo rotated">
    </div>
</template>

<style scoped lang="scss">
.img-bg-foot {
    width: 560px;
    height: 370px;
    overflow-y: hidden;

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
}
</style>