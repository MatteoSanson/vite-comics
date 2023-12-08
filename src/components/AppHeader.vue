<script>
import AppLogo from './AppLogo.vue';
import AppNavHeader from './AppNavHeader.vue';

export default {
    name: 'Header',
    components: {
        AppLogo,
        AppNavHeader,
    }
};
</script>

<template>
    <header>
        <div class="container">
            <AppLogo />
            <AppNavHeader />
        </div>
    </header>
</template>


<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;

header {
    color: $header;
}

.container {
    margin: 20px auto;
    width: 80%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>