<script>
export default {
    name: 'AppTitolo',
    props: {
        alt: String,
    }
};
</script>

<template>
    <div>
        <h4>{{ alt.toUpperCase() }}</h4>
    </div>
</template>

<style scoped lang="scss">
h4 {
    margin-top: 10px;
}
</style>