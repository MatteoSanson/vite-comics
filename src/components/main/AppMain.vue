<script>
import AppContentMain from './AppContentMain.vue';

export default {
    name: 'Main',
    components: {
        AppContentMain,
    }
};
</script>

<template>
    <main>
        <AppContentMain />
    </main>
</template>


<style scoped>
main {
    min-height: 500px;
    background-color: #1c1c1c;
    position: relative;
    overflow: hidden;
    color: white;

    &::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        height: 400px;
        background: url('/img/jumbotron.jpg') no-repeat center top / 100%;
        background-size: cover;
    }

}
</style>