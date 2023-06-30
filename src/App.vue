<script>
// Importo componenti 
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
// Importo il font 
import '@fontsource-variable/open-sans';
// Importo i data 
import MenuLinks from './assets/data/MenuLinks.js';

export default {
  // props: {
  //   MenuLinks
  // },
  components: {
    AppFooter,
    AppHeader,
    AppMain,
  },
  data() {
    return {
      navbarLinks: [
        {
          text: 'Characters',
          url: '#',
          current: false,
        },
        {
          text: 'Comics',
          url: '#',
          current: true,
        },
        {
          text: 'Movies',
          url: '#',
          current: false,
        },
        {
          text: 'TV',
          url: '#',
          current: false,
        },
        {
          text: 'Games',
          url: '#',
          current: false,
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false,
        },
        {
          text: 'Videos',
          url: '#',
          current: false,
        },
        {
          text: 'Fans',
          url: '#',
          current: false,
        },
        {
          text: 'News',
          url: '#',
          current: false,
        },
        {
          text: 'Shop',
          url: '#',
          current: false,
        },
      ],
      MenuLinks
    }

  }
}
</script>
<template>
  <AppHeader :links="navbarLinks" />
  <AppMain :menuLinks="MenuLinks" />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>