<script>
// Importo componenti 
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
// Importo il font 
import '@fontsource-variable/open-sans';
// Importo i data 
import MenuLinks from './assets/data/_menuLinks';
import NavbarLinks from './assets/data/_NavbarLinks';
import ComicBooks from './assets/data/_ComicBooks';

export default {
  components: {
    AppFooter,
    AppHeader,
    AppMain,
  },
  data() {
    return {
      MenuLinks,
      NavbarLinks,
      ComicBooks
    }

  }
}
</script>
<template>
  <AppHeader :links="NavbarLinks" />
  <AppMain :links="MenuLinks" />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>