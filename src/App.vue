<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppFooter from './components/AppFooter.vue';

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

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  color: $primary;
}
</style>
