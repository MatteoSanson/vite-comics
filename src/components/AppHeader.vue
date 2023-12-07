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
        <AppLogo />
        <AppNavHeader />
    </header>
</template>


<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;

header {
    color: $header;
}
</style>