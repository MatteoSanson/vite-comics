<script>
export default {
    name: 'AppCard',
    props: {
        image: String,
        title: String,
    }
};
</script>

<template>
    <li>
        <div class="img">
            <img :src="image" :alt="title">
        </div>
        <div>
            <h4>{{ title.toUpperCase() }}</h4>
        </div>
    </li>
</template>

<style scoped lang="scss">
li {
    width: calc(100% / 6 - 15px);
    margin-bottom: 20px;

    .img {
        margin: 0 auto;
        width: 100%;
        padding-top: 100%;
        overflow: hidden;
        position: relative;

        img {
            position: absolute;
            top: 0;
            left: 0;
            display: block;
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }

    h4 {
        margin-top: 10px;
    }
}
</style>