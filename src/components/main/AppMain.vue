<script>
import AppContentMain from './AppContentMain.vue';
import AppBgMain from './AppBgMain.vue';

export default {
    name: 'Main',
    components: {
        AppContentMain,
        AppBgMain,
    }
};
</script>

<template>
    <main>
        <AppBgMain />
        <AppContentMain />
    </main>
</template>


<style lang="scss">
main {
    background-color: #1c1c1c;
    display: flex;
    flex-direction: column;

    // min-height: 500px;
    // height: 100%;
    // background-color: #1c1c1c;
    // position: relative;
    // overflow: hidden;
    // color: white;

    // &::before {
    //     content: "";
    //     position: absolute;
    //     top: 0;
    //     left: 0;
    //     right: 0;
    //     height: 400px;
    //     background: url('/img/jumbotron.jpg') no-repeat center top / 100%;
    //     background-size: cover;
    // }

}
</style>