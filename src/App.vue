<script>
import AppHeader from './components/header/AppHeader.vue';
import AppMain from './components/main/AppMain.vue';
import AppJumbotron from './components/jumbotron/AppJumbotron.vue';
import AppFooter from './components/footer/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppJumbotron,
  },
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppJumbotron />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/partials/variables.scss' as *;
@use './styles/general.scss' as *;
</style>
