<script>
export default {
    name: 'Main',
};
</script>

<template>
    <main>

    </main>
</template>


<style scoped>
main {
    min-height: 500px;
    background-color: #1c1c1c;
    position: relative;
    overflow: hidden;

    &::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        height: 400px;
        background: url('../../../public/img/jumbotron.jpg') no-repeat center top / 100%;
        background-size: cover;
    }
}
</style>