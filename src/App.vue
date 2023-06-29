<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
// Supports weights 300-800
import '@fontsource-variable/open-sans';
export default {

  components: {
    AppFooter,
    AppHeader,
    AppMain,
  }
}
</script>
<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>